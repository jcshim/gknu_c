# 심재창의 첫 개인리포트
# 소감
- for 반복문에 대해서 이해 했음
- 이중 for에 대해서도 학습하였음
- C언어가 재미 있음
---
교수님 감사해요
--- 
  
```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);

    int h = n / 2;

    // 상단 (역삼각형)
    for (int i = 0; i <= h; i++) {
        for (int j = 0; j < i; j++) printf(" ");
        for (int j = 0; j < n - 2 * i; j++) printf("*");
        printf("\n");
    }

    // 하단 (삼각형)
    for (int i = h - 1; i >= 0; i--) {
        for (int j = 0; j < i; j++) printf(" ");
        for (int j = 0; j < n - 2 * i; j++) printf("*");
        printf("\n");
    }

    return 0;
}
```
