# InteractiveGuru
Applicants, students, facilitators and alumnis of our school can get information, tools, contacts and advice on everything Hyper and quick by asking an interactive guru.


var search = { "question": ["hey", "bro"], "answer": "It at least works man",
               "question": ["toilet", "wc"], "answer2": "you know where it is"};

var query = search.question;
var answer = search.answer;

console.log(query);
console.log(answer);

 $("#txt").keypress(function(e) {
   if(e.which == 13) {

    var str = $('#txt').val();

    if (query.some(function(v) { return str.indexOf(v) >= 0; })) {
      $('#result').html(answer);
      }
    else {
      $('#result').html('Bummer man! You just don\'t yap about Hyper, why are you even here dawg? ');
    }
}

  });

})(jQuery);
