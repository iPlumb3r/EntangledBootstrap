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
         <tr>            
             <td>Model</td>
             <td>Template, Ontology, ...</td>
             <td>Set of #Class, characterized by #Property & connected via #Relation</td>
             <td></td>
        </tr>
        </tr>
    </tbody>
</table>

Functional Modes
==
All required functions for the EBR (Cf next sections) are defined in order to be compliant with one or the other (or both) of the following functional mode : 
* Model-Driven Mode
* Model-Discovery Mode

Model-Driven Mode
-
It's a "top-down" mode, where the knowledge base management functionalities :    
* requires a pre-defined #Model in order to create/instanciate any #Individual   

This mode is appropriate when the knowledge domain is well-know and could be easily formalized   
=> This is the case for the __intentional aspect__ of the #Model (= #IntentionalModel)   

In this mode, the #KnowledgeBase is always coherent with the #Model

Model-Discovery Mode
-
It's a "bottom-up" mode, where the knowledge base management functionalities :   
* do NOT requires a pre-defined #Model in order to create/instanciate an #Individual.
* allows create an #Individual with no type (or typed "Thing")
* allows to change the type of an #Individual
* allows to multi-type an #Individual
* allows to defines "on-the-fly" new #Property & # Relation for a #Class

This mode is appropriate when the knowledge domain is NOT well defined ...
... and/or when the Ecosystem Mapping scope should be extended to an unknow new domain   
=> This is the case for the __extensional aspect__ of the #Model (= #EntensionalModel)

In this mode, it could appears incoherency #KnowledgeBase and the #Model, is NOT critical, ...   
... but those incoherencies should be easily detected, both : 
* At the #KnowledgeBase level, when some #Individual are characterised by #Property and/or #Relation not allowed at the #Model level
* At the #Model level, when news #Property and/or #Relation are used by some #Individuals   

=> This could permit the User to solve incoherencies, either by deleting "wrong" information at the #KnowledgeBase level, either by accepting new "rigth" constraints at the #Model level

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
This association allow the user to define characteristics (#Properties and/or #Relations) specified at #Class level for the new #Class   
Properties and/or relations not anymore compliants in the context of the news #Class are displayed in red or in another specific tab in order to be deleted (batch deletion feature appreciated)   

UF-05 : Associate a new #Class to an already "typed" #Individual (multi-typing)
-
Be able to associate an already "typed" #Individual to another #Class (in conjonction with the 1st one)   
Remark : Most of the time the 1st association is made with a #IntentionalClass ...   
... and the 2nd one is made with an #ExtensionalClass   
Associated #Properties and/or #Relations, should be diplay as followed : 
* #IntentionalClass characteristics (#Properties and/or #Relations), then #ExtensionalClass characteristics (#Properties and/or #Relations)
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
