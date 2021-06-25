function compressString(string) {
  let compressedString;
  for (let i = 0; i < string.length; ++) {
    if(i === i++) {
    let count = 0;
    let compressedString = `${count++}${i}`;
    }
  }
  return compressedString;
} 

//second solution with a while loop
function compressString(string) {
  let wordSize = string.length;
  let compressedWord;
  for (let i = 0; i < wordSize; ++) {
    let count = 0;
    while (i < wordSize - 1 && string[1] === string[i + 1]) {
      count++;
      i++;
      compressedWord = `${count}${i}`;
    }
  }
  return compressedWord;
}