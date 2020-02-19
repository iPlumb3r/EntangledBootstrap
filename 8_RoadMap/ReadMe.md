RoadMap
==
To Be Completed ...

Planned Releases
-
A list of planned releases for the EBR :   

<table>
    <thead>
        <tr>
            <th>V</th>
            <th>Name</th>
            <th>Model Scope</th>
            <th>Functional Mode</th>
            <th>Implementation type</th>
            <th>Target Technology</th>
            <th>Status</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>v0</td>
            <td>Proof Of Concept (PoC)</td>
            <td>Test Model</td>
            <td>Model-Driven (only)</td>
            <td>Centralized</td>
            <td>Topincs</td>
            <td>Current</td>
        </tr>
        <tr>
            <td>v1</td>
            <td>Minimum Viable Product (MVP)</td>
            <td>Intentional Model</td>
            <td>Model-Driven (only)</td>
            <td>Centralized</td>
            <td>Topincs</td>
            <td>In Design</td>
        </tr>
        <tr>
            <td>v2</td>
            <td>Full Viable Product (FVP)</td>
            <td>Full Model (Intentional + Extentional)</td>
            <td>Model-Driven & Model-Discovery</td>
            <td>Centralized</td>
            <td>The Networker</td>
            <td>In Study</td>
        </tr>
        <tr>
            <td>v3</td>
            <td>Final Product (FP)</td>
            <td>Full Model (Intentional + Extentional)</td>
            <td>Model-Driven & Model-Discovery</td>
            <td>Fully Distributed</td>
            <td>Holochain</td>
            <td>In Study</td>
        </tr>
    </tbody>
</table>

Model-Driven Mode
-
It's a "top-down" mode, where the knowledge base management functionalities :    
* requires a pre-defined #Model in order to create/instanciate any #Individual   

This mode is appropriate when the knowledge domain is well-know and could be easily formalized   
=> This is the case for the intentional aspect of the #Model (= #IntentionalModel)   

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
=> This is the case for the extensional aspect of the #Model (= #EntensionalModel)

In this mode, it could appears incoherency #KnowledgeBase and the #Model, is NOT critical, ...
... but those incoherencies should be easily detected, both : 
* At the #KnowledgeBase level, when some #Individual are characterised by #Property and/or #Relation not allowed at the #Model level
* At the #Model level, when news #Property and/or #Relation are used by some #Individuals
=> This could permit the User to solve incoherencies, either by deleting "wrong" information at the #KnowledgeBase level, either by accepting new "rigth" constraints at the #Model level
