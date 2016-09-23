=====================
Diagrame de structură
=====================

Diagrame de clasă
-----------------

Lista de atribute
^^^^^^^^^^^^^^^^^

.. code-block:: uml

   nume : tip atribut [= valoare implicită]

Lista de operații
^^^^^^^^^^^^^^^^^

.. code-block:: uml

   nume(lista de parametri) : tipul valorii returnate
   
Vizibilitate
^^^^^^^^^^^^

=====  =====
Symbol Semnif    
=====  =====
+      Public
#      Protected
-      Private 
~      Package
=====  =====

   
Moștenire 
^^^^^^^^^

Linie solidă din clasa copil (subclasa) la clasa părinte (superclasa) cu vîrf de săgeată neumplut.

Asociere [bidirecţională]
^^^^^^^^^^^^^^^^^^^^^^^^^

Linie solidă fără vîrf cu indicatori de cardinalitate la amble capete.

=====  =====
Indic  Semnif    
=====  =====
0..1   Zero sau unu
1      Unu
0..*   Zero sau mai mulți 
\*      Zero sau mai mulți
1..*   Unu sau mai mulți
n      Doar n
0..n   De la zero la n
n..m   De la n la m
=====  =====

Asociere [unidirecţională]
^^^^^^^^^^^^^^^^^^^^^^^^^

Linie solidă din clasa care deține relația (owner) la clasa care nu ''știe' de această relație cu vîrf de săgeată umplut (sau simplu). La capătul unde este vîrful se pune un indicator de cardinalitate.

Agregare
^^^^^^^^

Linie solidă din clasa parte (copil) la clasa întreg (părinte) cu vîrf în formă de diamant neumplut.

Compoziție
^^^^^^^^^^

La fel ca și relația de agregare doar că clasa copil nu poate exista decât în cazul existenţei clasei părinte. Se utilizează diamantul umplut.

Dependență (realizare)
^^^^^^^^^^^^^^^^^^^^^^

Linie întreruptă din clasa A la clasa B (astfel încît A are un atribut de tipul B) cu vîrf de săgeată neumplut (sau simplu).


Exemplu `Tutorial UML (partea a V-a). Class Diagram <http://www.techit.ro/tutorial_uml_5.php>`_
Exemplu `UML Class and Object Diagrams Overview <http://www.uml-diagrams.org/class-diagrams-overview.html>`_
Exemple avansate: `UML Class Diagrams Examples <http://www.uml-diagrams.org/class-diagrams-examples.html>`_

Exerciții `UML Exercises <https://lagunita.stanford.edu/c4x/DB/UML/asset/opt-uml.html>`_
Exerciții `Exercises on basic UML: structures<http://www.cs.unibo.it/~cianca/wwwpages/ids/esempi/uml-s.pdf>`_

Diagramă de componente
----------------------

Componenetele sistemului și legăturile dintre acesta.

Exemple `UML Component Diagrams Examples <http://www.uml-diagrams.org/component-diagrams-examples.html>`_

Diagrame structură composită
----------------------------

Structura internă a unei clase.

Exemple `UML Composite Structure Diagram Examples <http://www.uml-diagrams.org/composite-structure-examples.html>`_

Diagramă de Deployment
----------------------

Diagrame de obiecte
-------------------

Schemă `Object Diagram <http://www.uml-diagrams.org/class-diagrams-overview.html#object-diagram>`_

Exemple `Online Shopping Login Controller <http://www.uml-diagrams.org/online-shopping-user-login-uml-object-diagram-example.html>`_


Diagrame de pachete
-------------------

Atunci cînd se modelează un sistem cu multe elemente componente poate apărea necisitatea de a grupa elementele (dupa careva criterii) în pachete.

Exemple: `UML Package Diagram Examples <http://www.uml-diagrams.org/package-diagrams-examples.html>`_
