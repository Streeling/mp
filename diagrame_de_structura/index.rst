=====================
Diagrame de structură
=====================

Diagrame de clasă
=================

Lista de atribute
-----------------

.. code-block:: pascal

   <nume atribut> : <tip atribut> [= <valoare implicită>]

Lista de operații
-----------------

.. code-block:: uml

   <nume operație>(<lista de parametri>) : <tipul valorii returnate>
   
Vizibilitate
------------

====== ============
Symbol Semnificație
====== ============
`+`    Public
#      Protected
`-`    Private
`~`    Package
====== ============

Moștenire
---------

Relația de moștenire (sau generalizare) se reprezintă printr-o linie solidă din clasa copil (subclasa) la clasa părinte
(superclasa) cu vîrf de săgeată neumplut (triunghi).

Asociere [bidirecţională]
-----------------

Linie solidă cu sau fără vîrfuri (concomitent) cu indicatori de cardinalitate la amble capete.

========= ============
Indicator Semnificație
========= ============
0..1      Zero sau unu
1         Unu
0..*      Zero sau mai mulți
`*`       Zero sau mai mulți
1..*      Unu sau mai mulți
n         Doar n
0..n      De la zero la n
n..m      De la n la m
========= ============

Opțional:

* se poate adăuga deasupra liniei denumirea relației;
* se pot adăuga, la capetele liniei, atributele prin care se face asocierea (atributele se amplasează lîngă clasa care semnifică tipul acestuia).

Asociere [unidirecţională]
--------------------------

Linie solidă din clasa care deține relația (owner) la clasa care nu ''știe' de această relație cu vîrf de săgeată umplut (sau simplu). La capătul unde este vîrful se pune un indicator de cardinalitate.

Agregare
--------

Linie solidă din clasa parte (copil) la clasa întreg (părinte) cu vîrf în formă de diamant neumplut.

Compoziție
----------

La fel ca și relația de agregare doar că clasa copil nu poate exista decât în cazul existenţei clasei părinte. Se utilizează diamantul umplut.

Dependență
----------

Linie întreruptă din clasa A (sursa) la clasa B (ținta) cu vîrf de săgeată simplu. Semnificînd că A depinde de B, adică
dacă se schimbă B numaidecît va fi nevoie de operat schimbari sî în A. De regulă deasupra liniei se folosește un cuvînt
cheie care concretizează în ce constă dependența.

============= ============
Cuvînt cheie  Semnificația
============= ============
«call»        Clasa sursă apele una sau mai multe operați ale clasei țintă.
«create»      Clasa sursă crează exemplare ale clasei țintă.
«derive»
«instantiate» Clasa sursă este unexemplar al clasei țintă.
«permit»      Clasa țintă permite accesul clasei sursă la atribute private.
«realize»     Clasa sursă este o implemntare a interfeței țintă.
«refine»
«substitute»
«trace»
«use»         Clasa sursă are nevoie de clasa țintă în cadrul implemntării sale.
============= ============

Exemplu
-------

.. image:: class-diagram-domain-overview.png

Exerciții
---------

#. Analizați și descrieți diagrama `Library Domain Model <http://www.uml-diagrams.org/library-domain-uml-class-diagram-example.html>`_
#. Analizați și descrieți diagrama `Online Shopping <http://www.uml-diagrams.org/examples/online-shopping-domain-uml-diagram-example.html>`_
#. Construiți diagrama de clase pentru un serviciu web de poștă precum Gmail, Yahoo etc.

Diagramă de componente
======================

Componenetele sistemului și legăturile dintre acesta.

Exemple `UML Component Diagrams Examples <http://www.uml-diagrams.org/component-diagrams-examples.html>`_

Diagrame structură composită
============================

Structura internă a unei clase.

Exemple `UML Composite Structure Diagram Examples <http://www.uml-diagrams.org/composite-structure-examples.html>`_

Diagramă de deployment
======================

Afișează configurarea fizică a unui sistem. Aceste diagrame conțin noduri (sistem fizi sau un mediu software).
Iar fiecare nod poate conține fișiere (artefacet).

Diagrame de obiecte
===================

Diagrama obiect este o captură a obiectelor sistemului la un anumit moment. Diagramele obiect sînt utile în a exemplifica diagramele de clasă.

Schemă `Object Diagram <http://www.uml-diagrams.org/class-diagrams-overview.html#object-diagram>`_

Exemple `Online Shopping Login Controller <http://www.uml-diagrams.org/online-shopping-user-login-uml-object-diagram-example.html>`_

Diagrame de pachete
===================

Atunci cînd se modelează un sistem cu multe elemente componente poate apărea necisitatea de a grupa elementele (dupa careva criterii) în pachete.
În cazul diagramelor de pachete se pot folosi relațiile de dependență.


Exemple: `UML Package Diagram Examples <http://www.uml-diagrams.org/package-diagrams-examples.html>`_

Referințe
=========

#. `Tutorial UML (partea a V-a). Class Diagram <http://www.techit.ro/tutorial_uml_5.php>`_
#. `UML Exercises <https://lagunita.stanford.edu/c4x/DB/UML/asset/opt-uml.html>`_
#. `Exercises on basic UML: structures<http://www.cs.unibo.it/~cianca/wwwpages/ids/esempi/uml-s.pdf>`_
