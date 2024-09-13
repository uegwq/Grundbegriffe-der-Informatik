TARGET DECK
Grundbegriffe der Informatik

13 Auswertung einer Prädikatenlogischer Formel
---
Zuerst:
$\text{tval}_{D,I,\beta} : \text{Ter}^\Sigma \rightarrow D,$
Ordnet jedem Term ein Ergebnis aus dem Universum zu.
$\text{tval}_{D,I,\beta}(t) = \begin{cases}  \beta(x) & \text{falls } t = x \in \text{Var}_{\text{PL}} \\ I(f)(\text{tval}_{D,I,\beta}(t_1), \ldots, \text{tval}_{D,I,\beta}(t_k)) & \text{falls } t = f(t_1, \ldots, t_k), \text{ar}(f) = k \end{cases}$
Zu Formeln gibt es folgende Auswertungsfunktion:
$\text{val}_{D,I,\beta} : \text{For}_\Sigma \rightarrow \Bbb{B}$
(Es gelten dieselben Definitionen von $val_{AL}$ von [[Auswertungsfunktion]])
$\text{val}_{D,I,\beta}(R(t_1, \ldots, t_k)) = \begin{cases}  w & \text{falls } (\text{tval}_{D,I,\beta}(t_1), \ldots, \text{tval}_{D,I,\beta}(t_k)) \in I(R) \\ f & \text{falls } (\text{tval}_{D,I,\beta}(t_1), \ldots, \text{tval}_{D,I,\beta}(t_k)) \notin I(R)\end{cases}$
(Falls das keinen Sinn macht, mach dir klar, dass $I(R)$ die Menge aller Term-ar(R)-Tupel sind, für die R zu Wahr auswertet).
Es fehlen noch Quantoren:
Dafür musst du die [[Variablenbelegungsänderungsfunktion]] bissl verstanden haben. Es gilt:
$\text{val}_{D,I,\beta}(\forall x \ F) = \begin{cases}  w & \text{falls für jedes } d \in D \text{ und } \beta' = \beta^{d}_x \text{ gilt: } \text{val}_{D,I,\beta'}(F) = w \\ f & \text{sonst} \end{cases}$ $\text{val}_{D,I,\beta}(\exists x\ F) = \begin{cases}  w & \text{falls für (mind.) ein } d \in D \text{ und } \beta' = \beta^{d}_x \text{ gilt: } \text{val}_{D,I,\beta'}(F) = w \\ f & \text{sonst} \end{cases}$
<!--ID: 1707136930613-->

[[Prädikatenlogische Interpretation]]