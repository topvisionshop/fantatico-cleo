$(document).ready(function() {

	// Set URL with Tracker
	$('a').attr('href', trackerURL('https://ctrack.g2afse.com/click?pid=1444&offer_id=37'));
	$('a').on('click', function() {
		fbq('track', 'InitiateCheckout');
	});


	// Exit Event
	history.pushState({},"",location.href);
	history.pushState({},"",location.href);
	
	window.onpopstate = function(){
	setTimeout(function () {
	location.href = trackerURL('https://ctrack.g2afse.com/click?pid=1444&offer_id=37');
	},1);
	};

	var today = new Date();
	var dd = String(today.getDate()).padStart(2, '0');
	var mm = String(today.getMonth() + 1).padStart(2, '0'); //January is 0!
	var yyyy = today.getFullYear();
	
	today = dd + '/' + mm + '/' + yyyy;
	
    document.getElementById('dadata').innerHTML = today; 
});