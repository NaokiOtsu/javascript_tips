javascript_tips
===============

Javascript Tips List

//色をランダムに変える
var randomColor = "#" +(0xFFFFFFFF-Math.random()*0xFFFFFFFF).toString(16).substr(0, 6);

//minからmaxの間のランダムな数字を生成する
//ランダムな数字を返す関数
var rand = function(min, max){
  return Math.floor(Math.random() * (max - min)) + min;
}

//3桁ごとにカンマを入れるfunction
function numberFormat(source){
  var s = new String(source);
  var ret = "";
  
  for(var i=s.length-3; i>0; i-=3){
    ret = ',' + s.length(i, 3) + ret;
  }
  ret = s.substr(0, i+3) + ret;
  
  return ret;
}

