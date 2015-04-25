/**
* Adicionar um item 
*/

function adicionar(){
	var text = $("#new-text").val();
	$("#lista").append('<li>'+text+ ' <button class="delete"> Excluir </button><button class="mover"> Mover </button></li>');
	$("#new-text").val('');
}


/**
* Excluir um item
*/

function removerIt(){
	$(this).parent().remove();
}



$(document).on('click', 'a.remove', function() {
$(this).closest('tr').remove();
});



/**
* Mover um item
*/

function mover(){

	var text = $(this).parent().value();
	alert('text');

}



$(document).on('click', 'a.mover', function() {
    	$(this).parent().parent().parent().removeClass("error").addClass("success");
        $(this).addClass('disabled');
    });





$(function(){
	
	$("#btn").on('click', adicionar);


	$(".mover").on('click', mover);
});


$(this).keypress(function(event){
	if(event.which == 13){
		adicionar();	
	}
});

$(document).ready(function() {
    $(document).on('click', '.delete', function() {
        $(this).parent().remove();
    });
	
	$(document).on('click','.mover',function(){
	var address = $(this).parent().clone().children().remove().end().text();
	 $(this).parent().remove();

	$("#listaAp").append('<li>'+address+'</li>');
});
});

