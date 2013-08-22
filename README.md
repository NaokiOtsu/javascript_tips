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

