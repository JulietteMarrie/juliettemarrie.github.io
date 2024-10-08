<span style="font-size: 15px;"> $\begin{array}{ll} 
E_{\pi}[R_{t+1} + \gamma G_{t+1} | S_t = s] &= \sum\limits_{a} \pi(a|s) E_{\pi}[R_{t+1} + \gamma G_{t+1} | S_t = s, A_t = a]
\\ &= \sum\limits_{a} \pi(a|s) \sum\limits_{s'}\sum\limits_r p(s',r|s,a) E_{\pi}[R_{t+1} + \gamma G_{t+1} | S_t = s, A_t = a, S_{t+1}=s', R_{t+1}=r]
\\ &= \sum\limits_{a} \pi(a|s) \sum\limits_{s'}\sum\limits_r p(s',r|s,a) (r + \gamma E_{\pi}[G_{t+1} | S_{t+1}=s'] )
\end{array}$ </span>
