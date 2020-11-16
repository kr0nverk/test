```cpp
for(int i = 0; i < n; ++i) {
  C[i] = 0;
  for(int j = 0; i < n; ++j) {
    C[i] += A[i][j] * B[j];
  }
}
```
```cpp
for(int i = 0; i < n; ++i) {
  for(int j = 0; i < n; ++j) {
    C[i][j] = 0;
    for(int k = 0; k < n; ++k) {
      C[i][j] += A[i][k] * B[k][j];
    }
  }
}
```
```cpp
for(int i = 0; i < n; ++i) {
  for(int j = 0; i < n; ++j) {
    Bt[i][j] = B[j][i];
  }
}
for(int i = 0; i < n; ++i) {
  for(int j = 0; i < n; ++j) {
    C[i][j] = 0;
    for(int k = 0; k < n; ++k) {
      C[i][j] += A[i][k] * Bt[k][j];
    }
  }
}
```
