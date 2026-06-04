const searchInput = document.getElementById("searchInput");

searchInput.addEventListener("keyup", function(){

let filter = this.value.toLowerCase();

let cards = document.querySelectorAll(".card");

cards.forEach(card => {

let title = card.querySelector("h3").textContent.toLowerCase();

if(title.includes(filter)){
card.style.display = "block";
}else{
card.style.display = "none";
}

});

});

function openLogin(){
document.getElementById("loginModal").style.display="block";
}

function closeLogin(){
document.getElementById("loginModal").style.display="none";
}
