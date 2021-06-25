function compressString(string) {
  let compressedString;
  for (let i = 0; i < string.length; ++) {
    let count = 0;
    if(i === i++) {
    let compressedString = compressedString + `${count++}${i}`;
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
    while (i < wordSize - 1 && string[i] === string[i + 1]) {
      count++;
      i++;
      compressedWord = compressedWord + `${count}${i}`;
    }
  }
  return compressedWord;
}