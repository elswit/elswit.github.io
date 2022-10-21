---
title: "Design of high-order decoupled multirate GARK schemes"
collection: publications
permalink: /publication/MRGARK
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2009-10-01
venue: 'Journal 1'
paperurl: 'http://academicpages.github.io/files/paper1.pdf'
citation: 'Arash Sarshar, Steven Roberts, Adrian Sandu, Design of high-order decoupled multirate GARK
schemes, SIAM Journal on Scientific Computing, Vol. 41, No. 2, PP A816-A847.'
---
Multirate time integration methods apply different step sizes to resolve different components of the system based on the local activity levels. This local selection of step sizes allows increased computational efficiency while achieving the desired solution accuracy. While the multirate idea is elegant and has been around for decades, multirate methods are not yet widely used in applications. This is due, in part, to the difficulties raised by the construction of high order multirate schemes.
Seeking to overcome these challenges, this work focuses on the design of practical high-order multirate methods using the theoretical framework of generalized additive Runge-Kutta (MrGARK) methods, which provides the generic order conditions and the linear and nonlinear stability analyses.
A set of design criteria for practical multirate methods is defined herein: method coefficients should be generic in the step size ratio, but should not depend strongly on this ratio; unnecessary coupling between the fast and the slow components should be avoided; and the step size controllers should adjust both the micro- and the macro-steps.
Using these criteria, we develop MrGARK schemes of up to order four that are explicit-explicit (both the fast and slow component are treated explicitly), implicit-explicit (implicit in the fast component and explicit in the slow one), and explicit-implicit (explicit in the fast component and implicit in the slow one). Numerical experiments illustrate the performance of these new schemes.

[Download paper here](https://arxiv.org/abs/1804.07716)

Recommended citation: Your Name, You. (2009). "Paper Title Number 1." <i>Journal 1</i>. 1(1).
