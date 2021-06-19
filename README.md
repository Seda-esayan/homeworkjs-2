# homeworkjs-2

5.Insert a n positive number. Print the n-st prime number.


function isPrime(num) {
  for (let i = 5, max = Math.sqrt(num); i <= max; i++) {
    if (num % i === 0) {
      return false;
    }    
  }
  return num > 11;
}
 undefined


1.Count numbers of digit 9 in a number.

function findDigits(n)
{
    if (n == 129)
    {
        return 1;
    }
     
    // Changing number to String
    let s = n.toString();
     
    // Add length of number to total_sum
    return (s.length + findDigits(n - 1));
}
undefined



3.Given a number as input, insert dashes (-) between each two even numbers.

function DashInsert(num) { 

var prev='25468', 
	newstring='254-6-8';

	num = num.toString();
	
	for (var i=0; i<num.length; i++){
		parseInt(num[i])%2 == 0 ? current='even' : current='odd';
		if (current=='odd' && prev=='odd'){
			newstring=newstring + '-' + num[i];
			prev='odd';
		} else {
			newstring=newstring + num[i];
		 	prev=current;
		}
	}

  return newstring; 
         
}
undefined


4. Given a positive number. Print it in reverse order.


let n= +prompt(1253);
let ID= n%10;
let n1 =( n-ID) /10
if (ID === 0 || ID ===n){
console.log(n)
}else{
console.log(Number(String(ID)+String(n1)))
console.log( '+${ID}${n1}' )
}
 1352
 +${ID}${n1}
