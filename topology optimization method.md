# Definition of Topology
In design process, the topology usually is considered as a sub-field of geometry. The first work that related to topology was Königsberg bridge problem proposed by Euler. This problem was entitled "The solution of a problem relating to the geometry of position", which indicated that the distance was not relevant.[1] Etymologically, the word is derived from the Greek noun *topos* which means location, place, space or domain.[1] In mathematics, topology is concerned with a object that can be deformed, twisted, or stretched in an arbitrary manner.[2] If two objects have the same topology properties, they are said to be homeomorphic. 


# Topology optimization method

Optimize a topology, i.e. to arrange materials or position structures properly and make the objective reaches its global optimal. Therefore, topology optimization, differ from shape optimization, where only the shape of the boundary or of an interface of an object can be modified, also allow for the introduction of holes or structures thus for a change of the topology. This work will be concerned with topology optimization. 

Traditionally, it can be divided into two approaches, micro-structure topology optimization and marco-structure optimization. [3] 
## *Microstructure* 
In microstructure approaches, a fixed finite element mesh is used to describe the design domain. Typically the mesh is uniformly and rectangularly distributed in space, and the optimization is to determining whether the element of mesh is filled with materials or not. If a density is applied to represent the material, it is density method. If it only have a boolean value, i.e. 0 or 1, it is ON/OFF method. [6]

## *Marcostructure* 
Differ from microstructure approach, macrostructure approach does not work with a finite element mesh. Instead, it changes the boundaries of the design. 

In this class, solid isotropic materials are considered as opposed to porous, microstructured ones, and as the topology optimization is performed in conjunction with a shape optimization, the finite element mesh cannot be a fixed one, but must change with the changes of the boundaries of the design. Within the Macrostructure-approach, the topology of a solid body can be changed by growing or degenerating material or by inserting holes. The first method recognizes that an optimal design is simply a subset of the admissible design domain and that it can be obtained by appropriately adding or removing material from the admissible design domain, see 4,132,133,363. 

The second method mentioned consists of an iterative positioning of new holes "bubbles" at specific points in the topology domain. In each iteration, the holes and the existing variable boundaries of the continuous body are simultaneously subjected to a shape optimization procedure see 138,209,210,211,230,298.


## Topology Optimization Problem with pole number and coil winding arrangement 

In electric machine design process, the detailed distance and position of  specific structures are not very important. In initial design process, the combination of pole number and coil winding arrangement are more important. 

For the structure of Permanent Magnet Synchronous Motor(PMSM) design, the pole number and coil winding arrangement is a NP-complete problem. Topology Optimization Problem with pole number and coil winding arrangement is defined as follows:

Object function F: torque = 

subject to:
volume constraints: G_0<0
G_n<=0

the material distribution of copper and current direction is defined with a matrix:




**Detailed formula of pole number and coil winding arrangement in electric machine design**  



## Geometric topology optimization with polygons

For the purpose of solving the above-mentioned design problem in a numerically efficient way, the sensitivity-based topology algorithm was applied. The first definition of the topological gradient TG so-called bubble method originated from the work of Schumacher et al [9] 


A novel geometric topology optimization with polygons is introduced. This method is inspired by bubble method. Bubble method is a kind of geometric optimization method, and the idea of it was initially came from 0-1 check method, which is a kind of micro-structure optimization approaches.[4] [5][6] The basic idea  of proposed method is the iterative positioning of polygons into the present structure of component.

The optimization process is divided into the following steps (Fig. 3).

Step 1. For a given topology domain, shape optimization
is carried out, considering objective and constraint
functions, after which the structure of the component
in this topology class cannot be improved any
further.

Step 2. By inserting a hole (change of the topology class)
we try to achieve improved results. We require the
coordinates of the optimal position of the new hole
(bubble). The positioning is carried out via a hybrid algorithm combine multi-objective evolutionary algorithm and dynamic programming which determines the position of vertex set of polygon heuristically and analytically for objective and constraint functions.

Step 3. After the positioning, a shape optimization is carried
out in order to find the optimal shape of the new
bubbles and to determine the influence on the other
variable boundaries.

After the shape optimization has been completed, a further
bubble is inserted by means of the positioning criterion and
is then optimized with respect to its shape. This generates
an iterative process, and one obtains a number of possible
topologies out of which a suitable variant can be chosen by a
criterion still to be developed. The choice, in turn, must follow
external demands on the construction (e.g. possibilities
of manufacturing). 

## optimization method


As mentioned above, the electric machine topology design problem is very complex with numerous branches. Although the component is limited, but it can have countless connections. Therefore, it can be classified to a combinatorial optimization problem. Typically, combinatorial optimization problems can be viewed as searching for the best element of some set of discrete items; therefore, in principle, it is an NP-complete problem, which is one kind of search algorithm. Meta-heuristic can be used to solve them, for example, different kinds of  multi-objective evolutionary algorithm. However, generic search algorithms are not guaranteed to find an optimal solution, nor are they guaranteed to run quickly (in polynomial time). Since some discrete optimization problems are NP-complete, such as the traveling salesman problem, this is expected unless P=NP(which has not yet been proved).

In this project, we will use different kinds of meta-heuristic algorithm to solve the combinatorial optimization problem. 


[1]http://www-groups.dcs.st-and.ac.uk/history/HistTopics/Topology_in_mathematics.html\
[2]http://mathworld.wolfram.com/Topology.html\
[3] "Topology optimization of continuum structures:A review"\
[6](http://www.red.pe.org.pl/articles/2012/7a/58.pdf)\
[4]Bubble method for topology and shape optimization ofstructures (https://link.springer.com/content/pdf/10.1007%2FBF01742933.pdf) \
[5] Atrek, E. 1989: SHAPE: a program for shape optimization of
continuum structures. Proc. 1st Int. Conf. Opti'89, pp. 135-144.
Berlin, Heidelberg, New York: Springer 
[6]Bendsøe MP (1989) Optimal shape design as a material distribution
problem. Struct Optim 1:193–202