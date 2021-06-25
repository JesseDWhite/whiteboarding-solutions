function uniqueElements(string) {
  for (let i = 0; i < string.length; ++) {
    if(string.includes(i)) {
      return false;
    }
  }
  return true;
}