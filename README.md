# BUS353-Assignment-2-Noah_Beyerlein
Two Tab App
// this sets the background color of the master UIView (when there are no windows/tab groups on it)
Titanium.UI.setBackgroundColor('#000');

// create tab group
var tabGroup = Titanium.UI.createTabGroup();


//
// create base UI tab and root window
//
var win1 = Titanium.UI.createWindow({  
    title:'Noah Knows',
    backgroundImage:'NoahHoll_2873442b.png'
});
var tab1 = Titanium.UI.createTab({  
    icon:'KS_nav_views.png',
    title:'Noah Knows',
    window:win1
});

var label1 = Titanium.UI.createLabel({
	color:'#999',
	text:'The Rain is Coming! All creatures on the Ark',
	font:{fontSize:20,fontFamily:'Helvetica Neue'},
	textAlign:'center',
	width:'auto'
});

win1.add(label1);

//
// create controls tab and root window
//
var win2 = Titanium.UI.createWindow({  
    title:'Are you on the Ark?',
    backgroundImage:' Today.png '
});
var tab2 = Titanium.UI.createTab({  
    icon:'KS_nav_ui.png',
    title:'Are you on the Ark?',
    window:win2
});

var label2 = Titanium.UI.createLabel({
	color:'#999',
	text:'Pair up all creatures big and small!',
	font:{fontSize:20,fontFamily:'Helvetica Neue'},
	textAlign:'center',
	width:'auto'
});

win2.add(label2);



//
//  add tabs
//
tabGroup.addTab(tab1);  
tabGroup.addTab(tab2);  


// open tab group
tabGroup.open();

//Rotate Function
function rotatelayout() {
	win1.orientationModes = [Ti.UI.LANDSCAPE_RIGHT];
}
 tabGroup.open(); 
