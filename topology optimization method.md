# Topology optimization method

Optimize a topology, i.e. to arrange materials or position structures properly and make the whole object reaches it global optimal. Traditionally, it can be divided into mainly two approaches, micro-structure topology optimization and marco-structure optimization. [1]()


## *Microstructure* 
In microstructure approaches, a fixed finite element mesh is used to describe the design domain. Typically the mesh is uniformly and rectangularly distributed in space, and 
## *Marcostructure* 
Differ from microstructure approach, macrostructure approach does not work with a finite element mesh. Instead, it changes the boundaries of the design. 

In this class, solid isotropic materials are considered as opposed to porous, microstructured ones, and as the topology optimization is performed in conjunction with a shape optimization, the finite element mesh cannot be a fixed one, but must change with the changes of the boundaries of the design. Within the Macrostructure-approach, the topology of a solid body can be changed by growing or degenerating material or by inserting holes. The first method recognizes that an optimal design is simply a subset of the admissible design domain and that it can be obtained by appropriately adding or removing material from the admissible design domain, see 4,132,133,363. 

The second method mentioned consists of an iterative positioning of new holes "bubbles" at specific points in the topology domain. In each iteration, the holes and the existing variable boundaries of the continuous body are simultaneously subjected to a shape optimization procedure see 138,209,210,211,230,298.




[1]() "Topology optimization of continuum structures:A review"