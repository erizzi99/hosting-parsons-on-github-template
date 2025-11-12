---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Multiple Parson's Problems on One Page
---
# Java parson's problems

## Parsons 1 (Hello World)
Organizza i blocchi per stampare in output la stringa "Hello world"
<div id="hw-sortableTrash" class="sortable-code"></div> 
<div id="hw-sortableTrash" class="sortable-code"></div> 
<div id="hw-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="hw-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="hw-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "public class ProgHelloWorld{\n" + "    public static void main (String[] args){\n" + "        System.out.println(Hello World&quot;); \n" + "    }\n" + "}";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "hw-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
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

## Parsons 2 (Ciao a tutti)
Organizza i blocchi per stampare in output la stringa "Ciao a tutti" inserendo una parola per riga
<div id="ct-sortableTrash" class="sortable-code"></div> 
<div id="ct-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="ct-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="ct-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "System.out.print(&quot;Ciao&quot;);\n" + "System.out.println(&quot; &quot;); \n" + "System.out.print(&quot;a&quot;); \n" + "System.out.println(&quot; &quot;); \n" + "System.out.print(&quot;tutti&quot;);";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "ct-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#ct-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#ct-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 3 (Inizializzazione ed incremento #1)
Riordina i blocchi per inizializzare la variabile a, assegnarle il valore 5, incrementarla di 1 e stampare a video il suo valore
<div id="a1-sortableTrash" class="sortable-code"></div> 
<div id="a1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="a1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="a1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int a;\n" + "a = 5; \n" + "a = a + 1; \n" + "System.out.print(&quot;Valore di a: &quot;); \n" + "System.out.print(a);";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "a1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#a1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#a1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 4 (Inizializzazione ed incremento #2)
Riordina i blocchi per inizializzare la variabile a, assegnarle il valore 5, incrementarla di 1 e stampare a video il suo valore

<div id="a2-sortableTrash" class="sortable-code"></div> 
<div id="a2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="a2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="a2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int a = 5; \n" + "a += 1; \n" + "System.out.print(&quot;Valore di a: &quot;); \n" + "System.out.print(a);";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "a2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#a2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#a2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>



## Parsons 5 (Inizializzazione ed incremento #3)
Riordina i blocchi per inizializzare la variabile a, assegnarle il valore 5, incrementarla di 1 e stampare a video il suo valore



<div id="a3-sortableTrash" class="sortable-code"></div> 
<div id="a3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="a3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="a3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int a = 5; \n" + "a ++; \n" + "System.out.print(&quot;Valore di a: &quot;); \n" + "System.out.print(a);";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "a3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#a3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#a3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
