# quiz
const quiz = [
 {
   question:'俺の好きな食べ物は？',
   answers: [
   '豆腐',
   'ラーメン',
   'ガソリン',
   '焼き肉'
   ],
   correct: 'ラーメン'
 }, {
  question: '俺の好きな食べ物は？',
  answers: [
   '豆腐',
   'ラーメン',
   'ガソリン',
   '焼き肉'
 ],
correct: 'ラーメン'
}, {

  question: '俺の好きな食べ物は？',
  answers: [
   '豆腐',
   'ラーメン',
   'ガソリン',
   '焼き肉'
  ],
correct: 'ラーメン'
}, {

  question: '俺の好きな食べ物は？',
  answers: [
   '豆腐',
   'ラーメン',
   'ガソリン',
   '焼き肉'
  ],
  correct: 'ラーメン'
 }
];
const quizLength = quiz.length;
let quizIndex = 0;

const $button =  document.getElementsByTagName('button');
const buttonLength = $button.length;

const setupQuiz = () => {
	 document.getElementById('js-question').textContent = quiz[quizIndex];
	 let buttonIndex = 0;
	  while(buttonIndex < buttonLength){
	   $button[buttonIndex].textContent = quiz[quizIndex].answers[button]
	   buttonIndex++;
    }
}

setupQuiz();

const clickHandler = (e) => {
  if(quiz[quizIndex].correct === e.target.textContent){
	 window.alert('正解!!');
}   else {
	 window.alert('不正解......。');
}

quizIndex++;

if(quizIndex < quizLength){
	setupQuiz();
  }else {
	　window.alert('おわりー！！！')；
	}
}；

let handlerIndex = 0;
while (handlerIndex < buttonLegth){
	$button[handlerIndex].addEventListener('click',(e) => {
		clickHandler(e);
	});
	handlerIndex++; 
}




// $button[1].addEventListener('click', (e) => {
// 	clickHandler(e);
// });



// $button[2].addEventListener('click', (e) => {
// 	clickHandler(e);
// });


// $button[3].addEventListener('click', (e) => {
// 	clickHandler(e);
// });



// const question = '俺の好きな食べ物は？'
// const answers = [
//   '豆腐',
//   'ラーメン',
//   'ガソリン',
//   '焼き肉'
// ];

// const correct = 'ラーメン';
// const $button = document.getElementsByTagName('button');

// クイズの問題を文、選択肢を定義

//  let buttonIndex = 0;
//  let buttonLength = $button.length;
//  while(buttonIndex < buttonLength){
// 	$button[buttonIndex].textContent = answers[buttonIndex];
// 	buttonIndex++;
// }




  // document.getElementById('js-question').textContent = question;

  // document.getElementsByTagName('button')[0].textContent = answers[0];
  // document.getElementsByTagName('button')[1].textContent = answers[1];
  // document.getElementsByTagName('button')[2].textContent = answers[2];
  // document.getElementsByTagName('button')[3].textContent = answers[3];



// $button[0].textContent = answers[0];
// $button[1].textContent = answers[1];
// $button[2].textContent = answers[2];
// $button[3].textContent = answers[3];

//ボタンを押したら正誤判定
// while (handlerIndex)

// $button[0].addEventListener('click', (e) => {
// console.log(e);
// 	if(correct === e.target.textContent){
// 	 window.alert('正解!!');
// }   else {
// 	 window.alert('不正解......。');
// }

// });



// $button[1].addEventListener('click', (e) => {
// 	if(correct === e.target.textContent){
// 	window.alert('正解!!');
// }   else {
// 	window.alert('不正解......。');
// }

// });

// $button[2].addEventListener('click', (e) => {
// 	if(correct === e.target.textContent){
// 	window.alert('正解!!');
// }   else {
// 	window.alert('不正解......。');
// }

// });

// $button[3].addEventListener('click', (e) => {
// 	if(correct === e.target.textContent){
// 	window.alert('正解!!');
// }   else {
// 	window.alert('不正解......。');
// }

// });



// $button[0].addEventListener('click', () => {
// 	if(correct === $button[0].textContent){
// 	window.alert('正解!!');
// }   else {
// 	window.alert('不正解......。');
// }

// });

// $button[1].addEventListener('click', () => {
// 	if(correct === $button[1].textContent){
// 	window.alert('正解!!');
// }   else {
// 	window.alert('不正解......。');
// }

// });

// $button[2].addEventListener('click', () => {
// 	if(correct === $button[2].textContent){
// 	window.alert('正解!');
// }   else {
// 	window.alert('不正解......。');
// }

// });

// $button[3].addEventListener('click', () => {
// 	if(correct === $button[3].textContent){
// 	window.alert('正解!!');
// }   else {
// 	window.alert('不正解......。');
// }

// });


// document.getElementsByTagName('button')[0].addEventListener('click', () => {
// 	if (correct === document.getElementsByTagName('button')[0].textContent){
// 	window.alert('正解!!');}   //else {
// 	window.alert('不正解......。');}});

// document.getElementsByTagName('button')[1].addEventListener('click', () => {
// 	if (correct === document.getElementsByTagName('button')[1].textContent){
// 	window.alert('正解!!');}   else {
// 	window.alert('不正解......。');}});

// document.getElementsByTagName('button')[2].addEventListener('click', () => {
// 	if (correct === document.getElementsByTagName('button')[2].textContent){
// 	window.alert('正解!!');}   else {
// 	window.alert('不正解......。');}});

// document.getElementsByTagName('button')[3].addEventListener('click', () => {
// 	if (correct === document.getElementsByTagName('button')[3].textContent){
// 	window.alert('不正解.....。');}   else {
// 	window.alert('正解！！！！！');}});
