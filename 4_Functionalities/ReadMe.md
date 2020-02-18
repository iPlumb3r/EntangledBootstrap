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
            <td>A #Class allows to "type" an #Individual</td>
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
Remark : In this case the #Individual is "de facto" associated to the "root" #Class (= Thing)

This #Individual creation allow the user to define some key information about it :
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
This #Individual creation allow the user to define characteristics (properties and/or relations) specified at #Class level

UF-03 : Associate an existing #Individual to a #Class
-
Be able to associate an already existing #Individual (not already "typed") to a given #Class
This association allow the user to define new characteristics (properties and/or relations) specified at #Class level

UF-04 : Change the #Class of an already "typed" #Individual
-
Be able to associate an already "typed" #Individual to another #Class (instead of the 1st one)   
This association allow the user to define characteristics (properties and/or relations) specified at #Class level for the new #Class   
Properties and/or relations not anymore compliants in the context of the news #Class are displayed in red or in another specific tab in order to be deleted (batch deletion feature appreciated)   

UF-05 : Associate a new #Class to an already "typed" #Individual (multi-typing)
-
Be able to associate an already "typed" #Individual to another #Class (in conjonction with the 1st one)   
Remark : Most of the time the 1st association is made with a #IntentionalClass ...   
... and the 2nd one is made with an #ExtensionalClass   
Associated properties and/or relations, should be diplay as followed : 
* #IntentionalClass properties and/or relations, then #ExtensionalClass properties and/or relations
* Or, in separate tabs

Admin Functions
==

AF-01 : Create #Class
-
To Be Completed ...

AF-02 : Define #Class hierarchy
-
To Be Completed ...

AF-03 : Define #Class characteristics (#Properties & #Relations
-
To Be Completed ...
