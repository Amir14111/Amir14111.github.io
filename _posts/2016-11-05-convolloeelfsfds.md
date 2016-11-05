
$$
\delta_{m}^{l}\left(x,\: y\right)=\frac{\partial E}{\partial c_{m}^{l}\left(x,\, y\right)}=\sum_{o}\sum_{\, x',\, y'}^{N_{w},N_{w}}\underbrace{\frac{\partial E}{\partial c_{o}^{l+1}\left(x+x',\, y+y'\right)}}_{\delta_{o}^{l+1}\left(x+x',\, y+y'\right)}\cdot\frac{\partial c_{o}^{l+1}\left(x+x',\, y+y'\right)}{\partial c_{m}^{l}\left(x,\, y\right)}
$$

$$
\begin{aligned}

\frac{\partial c_{o}^{l+1}\left(x+x',\, y+y'\right)}{\partial c_{m}^{l}\left(x,\, y\right)} & =\frac{\partial}{\partial c_{m}^{l}\left(x,\, y\right)}\left(\sum_{m'}\sum_{\, x'',\, y''}^{N_{w},N_{w}}o_{m'}^{l}\left(x+x'-x'',\, y+y'-y''\right)\cdot w_{m',o}^{l+1}\left(x'',\, y''\right)\right)\\
 & =\frac{\partial}{\partial c_{m}^{l}\left(x,\, y\right)}\left(\sum_{m'}\sum_{\, x'',\, y''}^{N_{w},N_{w}}a\left(c_{m'}^{l}\left(x+x'-x'',\, y+y'-y''\right)\right)\cdot w_{m',o}^{l+1}\left(x'',\, y''\right)\right)\\
 & =\frac{\partial}{\partial c_{m}^{l}\left(x,\, y\right)}\left(w_{0,o}^{l+1}\left(0,\,0\right)\cdot a\left(c_{0}^{l}\left(x'-0,\, y'-0\right)\right)+\ldots+w_{m,o}^{l+1}\left(x'',\, y''\right)\cdot a\left(c_{m}^{l}\left(x,\, y\right)\right)+\ldots\right)\\
 & =w_{m,o}^{l+1}\left(x+x',\, y+y'\right)\cdot\frac{\partial a\left(c_{m}^{l}\left(x,\, y\right)\right)}{\partial c_{m}^{l}\left(x,\, y\right)}

\end{aligned}
$$

$$
\delta_{m}^{l}\left(x,\: y\right)=\underbrace{\sum_{o}\sum_{\, x',\, y'}^{N_{w},N_{w}}\delta_{o}^{l+1}\left(x+x',\, y+y'\right)\cdot w_{m,o}^{l+1}\left(x',\, y'\right)}_{\text{Cross-Correlation, Backpropagated Error}}\cdot\frac{\partial a\left(c_{m}^{l}\left(x,\, y\right)\right)}{\partial c_{m}^{l}\left(x,\, y\right)}
$$