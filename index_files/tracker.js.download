// Get URL params
function getUrlParameter(sParam) {
    var sPageURL = decodeURIComponent(window.location.search.substring(1)),
        sURLVariables = sPageURL.split('&'),
        sParameterName,
        i;

    for (i = 0; i < sURLVariables.length; i++) {
        sParameterName = sURLVariables[i].split('=');

        if (sParameterName[0] === sParam) {
            return sParameterName[1] === undefined ? true : sParameterName[1];
        }
    }
}

// Give the URL parameters variable names
var pixel = getUrlParameter('pixel');
var adv = getUrlParameter('adv');
var src = getUrlParameter('src');

function trackerURL(url) {
	url += "&sub1=" + src;
	url += "&sub2=" + adv;
	url += "&sub4=" + pixel;
 	
 	// Return URL
	return url;
}
