Functionalities
==
To Be Completed ...

Glossary
-
<table>
    <thead>
        <tr>
            <th>Prefered Label</th>
            <th>Alternative(s) Label(s)</th>
            <th>Description</th>
            <th>Comment</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Individual</td>
            <td>Individu, Instance, Topic, ...</td>
            <td>(Tangible or Intangible) Element of the real world</td>
            <td></td>
        </tr>
        <tr>
            <td>Class</td>
            <td>Universal, Category, Topic Type, ...</td>
            <td>Set of #Individual who are sharing the same characteristics : #Property and/or #Relation (between others elements)</td>
            <td></td>
        </tr>
        <tr>
            <td>Property</td>
            <td>Attribute, Occurence, ...</td>
            <td>Characteristic of a #Class</td>
            <td>Domain of characteristic are mostly textual or numeric</td>
        </tr>
        <tr>
            <td>Relation</td>
            <td>Association, Link, ...</td>
            <td>Connection between 2 (or several) #Class</td>
            <td></td>
        </tr>
    </tbody>
</table>


User Functions
==

UF-01 : Basic #Individual creation
-
Be able to create a #Individual without having to specify for it a given specific #Class   
(In this case the #Individual is "de facto"  associated to the "root" #Class "Thing")

This #Individual creation allow the user to define some key information about it
<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Range</th>
            <th>Min Card</th>
            <th>Max Card</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Prefered Label</td>
            <td>Property</td>
            <td>Text</td>
            <td>1</td>
            <td>1</td>
        </tr>
        <tr>
            <td>Alternative Label</td>
            <td>Property</td>
            <td>Text</td>
            <td>0</td>
            <td>N</td>
        </tr>
        <tr>
            <td>Description</td>
            <td>Property</td>
            <td>Text</td>
            <td>0</td>
            <td>1</td>
        </tr>
        <tr>
            <td>Comment</td>
            <td>Property</td>
            <td>Text</td>
            <td>0</td>
            <td>N</td>
        </tr>
        <tr>
            <td>Home Page</td>
            <td>Property</td>
            <td>URL</td>
            <td>0</td>
            <td>1</td>
        </tr>
        <tr>
            <td>About Page</td>
            <td>Property</td>
            <td>URL</td>
            <td>0</td>
            <td>N</td>
        </tr>
        <tr>
            <td>Documented By</td>
            <td>Relation</td>
            <td>#Document</td>
            <td>0</td>
            <td>N</td>
        </tr>
    </tbody>
</table>

UF-02 : Advanced #Individual creation
-
Be able to create a #Individual while associating it to a given #Class   
This #Individual creation allow the user to define informations specified at #Class level

UF-03 : Associate an existing #Individual to a #Class
-
Be able to associate an already existing #Individual (not typed) to a given #Class

Admin Functions
==

AF-01
-
Text text ...

AF-02
-
Text text ...

AF-03
-
Text text ...
