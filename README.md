```cpp
for(int i = 0; i<n; ++i) {
  c[i] = 0;
  for(int j = 0; i<n; ++j) {
    c[i] += A[i][j] * b[j];
  }
}
```
```cpp
for(int i = 0; i<n; ++i) {
  for(int j = 0; i<n; ++j) {
    c[i][j] = 0;
     for(int k = 0; k<n; ++k) {
      c[i][j] += A[i][k] * B[k][j];
  }
  }
}
```
