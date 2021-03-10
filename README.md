# US2BPMN

Transformation des User stories vers BPMN utilisant henshin

<h2>Transformations opérationnelles: </h2>
<ul>
  <li>initModel(BacklogId,name) </li>
  <li>Creation des activitées : tasks(BacklogId,name) </li>
  <li>Creation des start/END Events:StartEvent(name,?) && EndEvent(?,name)</li>
  <li>Creation des Sequences Flow: CreateSequenceFlow(?,?,name)</li>
</ul>

<h2>Transformations implémentées mais non opérationnelles:</h2>
   <li>Creations des evenements: ComplexGatway+ExclusiveGatway+InclusiveGatway+ParallelGatway</li>
<h2>Exécution</h2>
   
   <li>Structure</li>
   <ul>
   <li>ouvrirUS2BPMN.henshin_diagram</li>
    <p>US_TO_BPMN -> model -> Transformations -> ouvrir US2BPMN.henshin_diagram</p>
   <li>executer mainUnit</li>
      <p>cliquer à droite sur MainUnit ->apply transformation</p>
      <p>saisir Input model (>US_TO_BPMN/model/US_meta/UserStories.xmi)</p>
      <p>saisir parameters: dans notre cas BacklogId="UserID" && name="User"</p>
      <p>Transform: un fichier destination est généré (US_TO_BPMN/model/US_meta/UserStories_transformed.xmi) </p>
   </ul>
  
