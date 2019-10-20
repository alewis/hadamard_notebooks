Mathematica notebooks to manipulate bispinor and bitensor quantities.
The initializations are in BispinorCoincidenceInitialize.nb. StressTensorHadamardDivergences.nb computes the divergences of
the stress-energy tensor along with some other operators. geodexpand.nb and sigexpand.nb implement specializations to a conformally
flat chart. ComputeSigmaCoincidenceLimits.nb and ComputeVanVleckCoincidenceLimits4D.nb show how to compute coincidence limits of 
the world function and van Vleck determinant, respectively.

These notebooks are based on xAct, xTensor, and xTras, http://xact.es/xTensor/. I didn't end up using Spinors (the package), since it's 
specialized to 4D, and since I had enough conceptual trouble connecting the Penrose spinor language used there to the
``standard QFT" Dirac spinors in 2D that I needed that writing my own stuff seemed easier. But if you are working in 4D, I would
recommend you use Spinors, because it's much better documented and tested.

I have successfully used these functions to:
    -Compute coincidence limits of bispinors, bitensors, and their derivatives, by successively differentiating a PDE that defines them.
    -Commute covariant derivatives that mix spinor and tensor indices at two different points (each point is implemented as a different manifold).
    -Isolate the divergent and finite terms in equations involving bispinors and bitensors. In particular, the divergent and finite
     terms of the stress-energy tensor of a 2D Dirac field. A higher-dimension Dirac field would not be much harder.

These notebooks have not been tested in any disciplined way, even on my own laptop. I would be very surprised if they were unsafe, but no
guarantees. They almost certainly contain bugs, though.

I will at some point come back here to refactor and document these notebooks in a manner that is comprehensible to others. Until then,
if you would like to use these, please get in touch at adam.lws@(Google's email service). 

Should you use these to obtain a result that you publish, I'd be thrilled if you cited https://arxiv.org/abs/1910.05663.

