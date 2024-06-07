# Resume_Builder
This project is a dynamic and user-friendly resume builder implemented using React JS. It empowers users to effortlessly create and edit their resumes with a live preview feature, making the process seamless and intuitive. The project also includes additional features to enhance the user experience.

# Currently Under Development
![Under_Development](Resume_Template/Construction.png) 
- Stay Tuned For More Updates

## Upcoming Features

### 1. User-friendly Interface

The project provides an intuitive and easy-to-use interface for creating and editing resumes. Users can navigate seamlessly through the platform, ensuring a smooth experience.

### 2. Live Resume Preview

As users fill in their details in the text boxes, the changes are reflected in real-time on the selected resume template displayed on the right side of the screen. This live preview feature enables users to visualize the final result as they input information.

### 3. Resume Templates

The platform offers a variety of resume templates tailored for different job industries. Users can choose a template that aligns with their preferences and the industry they are targeting.

### 4. PDF Export

Once users have completed their resume, they have the option to export it as a PDF document. This functionality ensures that users can easily share or print their resumes in a professional format.

### 5. Dark Mode

The project includes a dark mode feature to enhance viewing comfort, especially during extended usage periods. Users can toggle between light and dark modes based on their preferences.

### 6. Image Upload for Profile Picture

Users can personalize their resumes by uploading a profile picture. This feature adds a personal touch to the resume and helps create a professional and visually appealing document.


5..

#include <stdio.h>

int main() {
    int n, sum = 0;
    printf("Enter the number of terms: ");
    scanf("%d", &n);
    for (int i = 1; i <= n; i++) {
        sum += i;
        printf("%d ", sum);
    }
    return 0;
}


6..

#include <stdio.h>

int main() {
    int n, num, sum_odd = 0, sum_even = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d numbers: ", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        if (arr[i] % 2 == 0) {
            sum_even += arr[i];
        } else {
            sum_odd += arr[i];
        }
    }
    printf("Sum of even numbers: %d\n", sum_even);
    printf("Sum of odd numbers: %d\n", sum_odd);
    return 0;
}


7..

#include <stdio.h>

int main() {
    for (int i = 151; i < 445; i += 2) {
        if (i % 7 == 0 && i % 3 != 0) {
            printf("%d ", i);
        }
    }
    return 0;
}


8..

#include <stdio.h>

int main() {
    FILE *source, *target;
    char ch;
    
    source = fopen(__FILE__, "r");
    if (source == NULL) {
        printf("Source file not found\n");
        return 1;
    }
    
    target = fopen("code.txt", "w");
    if (target == NULL) {
        printf("Error opening target file\n");
        return 1;
    }
    
    while ((ch = fgetc(source)) != EOF) {
        fputc(ch, target);
    }
    
    printf("File copied successfully.\n");
    fclose(source);
    fclose(target);
    return 0;
}


9..

#include <stdio.h>

int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n], unique[n], k = 0;
    
    printf("Enter %d numbers: ", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    for (int i = 0; i < n; i++) {
        int j;
        for (j = 0; j < k; j++) {
            if (arr[i] == unique[j])
                break;
        }
        if (j == k) {
            unique[k++] = arr[i];
        }
    }
    
    printf("Array after removing duplicates: ");
    for (int i = 0; i < k; i++) {
        printf("%d ", unique[i]);
    }
    return 0;
}


10..

#include <stdio.h>

int main() {
    int size;
    char ch;
    printf("Enter the size of square: ");
    scanf("%d", &size);
    printf("Enter the character: ");
    scanf(" %c", &ch);
    
    for (int i = 0; i < size; i++) {
        for (int j = 0; j < size; j++) {
            if (i == 0 || i == size - 1 || j == 0 || j == size - 1) {
                printf("%c ", ch);
            } else {
                printf("  ");
            }
        }
        printf("\n");
    }
    return 0;
}


12. ..
#include <stdio.h>

int main() {
    int num1, num2;
    printf("Enter two integers: ");
    scanf("%d %d", &num1, &num2);
    
    int last_digit_sum = (num1 % 10) + (num2 % 10);
    
    printf("Sum of last digits: %d\n", last_digit_sum);
    return 0;
}


13..
#include <stdio.h>

int main() {
    int a, b, c;
    printf("Enter three integers: ");
    scanf("%d %d %d", &a, &b, &c);
    
    int max = a > b ? (a > c ? a : c) : (b > c ? b : c);
    int min = a < b ? (a < c ? a : c) : (b < c ? b : c);
    int mid = a + b + c - max - min;
    
    printf("Ascending order: %d %d %d\n", min, mid, max);
    return 0;
}


14..
#include <stdio.h>

int main() {
    int num;
    printf("Enter a positive number: ");
    scanf("%d", &num);
    
    printf("The number %d is ", num);
    num & 1 ? printf("odd.\n") : printf("even.\n");
    return 0;
}

15..

#include <stdio.h>
#include <string.h>

int main() {
    char str[100];
    printf("Enter a string: ");
    scanf("%s", str);
    
    int len = strlen(str);
    for (int i = 0; i < len; i++) {
        for (int j = 0; j <= i; j++) {
            printf("%c", str[j]);
        }
        printf("\n");
    }
    return 0;
}


