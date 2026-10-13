layout: default
title: Multiple Parson's problems in C
## HELLO WORLD
<div id="hw-sortableTrash" class="sortable-code"></div> 
<div id="hw-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="hw-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="hw-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = `#include \u003cstdio.h\u003e
int main() {
    printf("Hello World!\\n");
    return 0;
}`;
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "hw-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#hw-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#hw-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
## INPUT DI UN DATO INTERO
<div id="id-sortableTrash" class="sortable-code"></div> 
<div id="id-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="id-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="id-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = `#include \u003cstdio.h\u003e
int main() {
    int numero;
    printf("Inserisci un numero intero: ");
    scanf("%d", &numero);
    printf("Hai inserito: %d", numero);
    return 0;
}`;
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "id-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#id-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#id-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
