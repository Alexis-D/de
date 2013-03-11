This is a quick implementation of differential evolution (Storn & Price, 1997) in Python 3. You should check out their paper _Differential evolution-a simple and efficient heuristic for global optimization over continuous spaces_ it's really well written and interesting.

You can see a quick example of how to use it at the bottom of de.py. It tries to minimize the Ackley function and show the results of DE for different numbers of iterations.

There are also a few TODOs that I may or may not do (this implementation was mostly made for fun rather than for real use...).

You can also take a look at the output of `pydoc`.

    Help on module de:
    
    NAME
        de
    
    DESCRIPTION
        # -*- coding: utf-8 -*-
        # TODO(alexis): add **tests** (and try unittest.mock.MagicMock at the same
        # time).
    
    CLASSES
        builtins.object
            DE
        
        class DE(builtins.object)
         |  This class implements differential evolution.
         |  
         |  This method is described by Storne and Price in a paper titled
         |  "Differential evolution-a simple and efficient heuristic for global
         |  optimization over continuous spaces".
         |  
         |  Variables names in the implementation (x, y, z, u, v, F, CR, NP) try to
         |  match their equivalents in the paper.
         |  
         |  Methods defined here:
         |  
         |  __init__(self, x='rand', y=1, z='bin', *, F=0.5, CR=0.1)
         |  
         |  solve(self, fitness, initial_population, iterations=1000)
         |      # TODO(alexis): add a fitness_aim param?
         |      # TODO(alexis): add a generic way to generate initial pop?
         |  
         |  ----------------------------------------------------------------------
         |  Data descriptors defined here:
         |  
         |  CR
         |      Weight used during bin crossover.
         |  
         |  F
         |      Weight used during mutation.
         |  
         |  __dict__
         |      dictionary for instance variables (if defined)
         |  
         |  __weakref__
         |      list of weak references to the object (if defined)
         |  
         |  x
         |      How to choose the vector to be mutated.
         |  
         |  y
         |      The number of difference vectors used.
         |  
         |  z
         |      Crossover scheme.
    
    DATA
        __all__ = ['DE']
    
    FILE
        /home/alexis/de/de.py
    
    
