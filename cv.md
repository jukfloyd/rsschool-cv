# Aleksei Zhuchkov

## Contacts

Mob.: +7-929-930-09-06  
E-mail: zhuchkovav@gmail.com

## About me

I started working on internet projects since 2000 as a programmer. Last 4 years I am a head of digital support. I want to renew my programming skills.

## Skills

* Perl, PHP, MySQL (Linux platforms)
* C#, MS SQL (Windows platforms)
* HTML, CSS, Javascript

## Code exmaples

```
function spiralize(N) {
  if (N < 1 || parseInt(N) != N || typeof N != 'number') return [];
  let matrix = (N == 1) ? [[]] : [...Array(N)].map(item => [...Array(N)].map(item => 0));
  const fN = Math.floor(N/2);
  for (let n=0; n<fN; n++) {
    let iL = N-n*2*2;
    if (iL == 1) {
      matrix[fN][fN] = 1;
    }
    for (let i = 1; i<= (iL-1)*4; i++) {
      if (i >= 1 && i <= iL)
        matrix[0+n*2][i-1+n*2] = 1;
      if (i > iL && i <= (iL-1)*2)
        matrix[i-iL+n*2][N-1-n*2] = 1;
      if (i > (iL-1)*2 && i <= (iL-1)*3 + 1) {
        if (i == (iL-1)*3 + 1 && iL == 2) break;
        matrix[N-1-n*2][iL*3-2-i+n*2] = 1;
      }
      if (iL > 2) {
        if (i > (iL-1)*3 + 1 && i <= (iL-1)*4-1) 
          matrix[(iL-1)*4-i+n*2+1][n*2] = 1;
        if (i == (iL-1)*4-1 && iL > 4) 
          matrix[(iL-1)*4-i+n*2+1][n*2+1] = 1;
      }
    }
  }
  return matrix;
}
```

## Experience

6-years of Perl-programming  
5-years of C# programming  
5-years of PHP-programming  
Unfortunately all my projects since 2000 are closed by now...

## Education

High Education, MSTU n.a. Baumann

## Language

English, Intermediate