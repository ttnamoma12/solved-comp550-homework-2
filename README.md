Download Link: https://assignmentchef.com/product/solved-comp550-homework-2
<br>
<strong>Algorithmic Robotics</strong>




Please read the honor code and the additions described in the course syllabus. Present your work and your work only. You must <em>explain </em>all of your answers. Answers without explanation will be given no credit.

<ol>

 <li>(20 points) A set <em>S </em>and an operator form a <em>group </em>if the following properties are satisfied:</li>

</ol>

Closure        For all <em>s</em><sub>1 </sub>and <em>s</em><sub>2 </sub>in <em>S</em>, <em>s</em><sub>1</sub>·<em>s</em><sub>2 </sub>is also an element of <em>S</em>.

Associativity            For all <em>s</em><sub>1</sub>, <em>s</em><sub>2 </sub>and <em>s</em><sub>3 </sub>in <em>S</em>, (<em>s</em><sub>1</sub>·<em>s</em><sub>2</sub>)·<em>s</em><sub>3 </sub>= <em>s</em><sub>1</sub>·(<em>s</em><sub>2</sub>·<em>s</em><sub>3</sub>).

Identity              There exists an element of <em>S </em>denoted by <em>I </em>such that <em>I</em>·<em>s</em><sub>1 </sub>= <em>s</em><sub>1</sub>·<em>I </em>= <em>s</em><sub>1 </sub>for all <em>s</em><sub>1 </sub>in <em>S</em>.

Inverse         For each <em>s</em><sub>1 </sub>there exists a <em>s</em><sub>2 </sub>in <em>S </em>such that <em>s</em><sub>1</sub>·<em>s</em><sub>2 </sub>= <em>s</em><sub>2</sub>·<em>s</em><sub>1 </sub>= <em>I</em>.

Let T be the set of all rigid body transformations in 2D in homogeneous coordinates. Prove that T and regular matrix multiplication form a <em>group</em>. That is, prove that T and regular matrix multiplication satisfy the properties listed above. In your answers, use the facts that:

<ul>

 <li>Rotation matrices with matrix multiplication form a group.</li>

 <li>Translation vectors and vector addition form a group.</li>

</ul>

In your answers, you can write a rigid body transformation:

<em>T<sub>i </sub></em>

<ol start="2">

 <li>(10 points)

  <ul>

   <li>(5 points) What is a rotation of radians about the axis [0 0 1]<em><sup>T </sup></em>as a unit quaternion, <em>q</em><sub>1</sub>?.</li>

   <li>(5 points) Given the quaternion <em>q</em><sub>2 </sub>= 0+1<em>i</em>+0<em>j</em>+0<em>k</em>, what is <em>q</em><sub>1 </sub><em>q</em><sub>2</sub>? Here, “·” is quaternion multiplication.</li>

  </ul></li>

 <li>(15 points)</li>

</ol>

Figure 1: From left to right: a manipulator with two prismatic joints, a manipulator with three revolute joints, and a manipulator with two revolute joints and a prismatic joint.

For each of the three manipulators shown in Figure ??, determine the topology and dimension of the manipulator’s configuration space.

<ol start="4">

 <li>(30 points) Figure ?? shows a three-link kinematic chain in 2D. The lengths of link <em>A</em><sub>1</sub>, <em>A</em><sub>2 </sub>and <em>A</em><sub>3 </sub>are <em>l</em><sub>1</sub>, <em>l</em><sub>2 </sub>and <em>l</em><sub>3</sub>, respectively. The joint angles of the chain are <em>θ</em><sub>2 </sub>and <em>θ</em><sub>3</sub>, as shown in Figure ??. For each link, we attach a local frame to the base end of that link (e.g., for link <em>A</em><sub>1</sub>, the axes of frame 1, <em>x</em><sub>1 </sub>and <em>y</em><sub>1 </sub>are labeled).</li>

</ol>

Figure 2: The Three-Link Chain

<ul>

 <li>(5 points) Determine the topology and dimension of the configuration space for this manipulator.</li>

 <li>(5 points) Determine the Homogeneous coordinates <em>v</em><sub>3 </sub>of the point 2 in the local frame of link <em>A</em><sub>3</sub>, in terms of <em>l</em><sub>1</sub>, <em>l</em><sub>2</sub>, <em>l</em><sub>3</sub>, <em>θ</em><sub>2 </sub>and <em>θ</em><sub>3</sub>.</li>

 <li>(5 points) Determine the forward kinematics of this three-link chain. That is, calculate the homogeneous coordinates <em>v</em><sub>1 </sub>of the point 2 in the local frame of link <em>A</em><sub>1</sub>, in terms of <em>l</em><sub>1</sub>, <em>l</em><sub>2</sub>, <em>l</em><sub>3</sub>, <em>θ</em><sub>2 </sub>and <em>θ</em><sub>3</sub>.</li>

 <li>(5 points) Determine the homogeneous transformations from the local frame of <em>A</em><sub>3 </sub>to the local frame of <em>A</em><sub>1</sub>. That is, determine the transformation matrices <em>T</em><sub>2 </sub>and <em>T</em><sub>3 </sub>such that, <em>T</em><sub>2 </sub>moves <em>A</em><sub>2 </sub>from its local frame to the local frame of <em>A</em><sub>1</sub>, and <em>T</em><sub>3 </sub>moves <em>A</em><sub>3 </sub>from its local frame to the local frame of <em>A</em><sub>2</sub>. Then the transformation matrix <em>T</em><sub>2</sub><em>T</em><sub>3 </sub>moves <em>A</em><sub>3 </sub>from its local frame to the local frame of <em>A</em><sub>1</sub>.</li>

 <li>(10 points) Show that <em>v</em><sub>1 </sub>= <em>T</em><sub>2</sub><em>T</em><sub>3</sub>·<em>v</em><sub>3</sub>.</li>

</ul>

<ol start="5">

 <li>(15 points) Consider workspace obstacles A and B. If A∩B 6= 0/, do the configuration space obstacles QA and QB always overlap? If A ∩ B = 0/, is it possible for the configuration space obstacles QA and QB to overlap? Justify your claims for each question.</li>

 <li>(10 points) Suppose five polyhedral bodies float freely in a 3D world. They are each capable of rotating and translating. If these are treated as “one” composite robot, what is the topology of the resulting configuration space (assume that the bodies are not attached to each other)? What is the dimension of the composite configuration space?</li>

</ol>

2