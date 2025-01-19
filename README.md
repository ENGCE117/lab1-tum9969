## ข้อบังคับ
1. ต้องกรอกรายละเอียดของตนเองในไฟล์ `student_info.txt` โดยมีข้อมูลสำคัญที่ต้องกรอกคือ
   - รหัสนักศึกษา เช่น 678888888-8
   - รหัสวิชา เช่น ENGCE117
   - เทอมที่เรียน เช่น 2/2567
2. นักศึกษาต้องทำการเขียนโค้ดโปรแกรมที่ไฟล์ `student_program.cpp` 

## โจทย์
จงเขียนรายละเอียดของฟังก์ชันจาก Prototype ต่อไปนี้
- ฟังก์ชัน GetMatrix เพื่อรับค่าจากผู้ใช้ 2 ค่า เพื่อทำการกำหนดค่าภายใน Matrix 2 มิติ และรับค่าจากผู้ใช้เพื่อกำหนดค่าภายใน Matrix
- ฟังก์ชัน PrintMatrix เพื่อแสดงค่าทั้งหมดที่อยู่ภายใน Matrix

## FIX CODE
```c++
#include <stdio.h>

void GetMatrix( int **value, int *row, int *col ) ;
void PrintMatrix( int **value, int row, int col ) ;

int main() {
    int *data, m = 3, n = 3 ;
    data = new int[ m * n ] ;
    GetMatrix( &data, &m, &n ) ;
    PrintMatrix( &data, m, n ) ;
    return 0 ;
}//end function
```

## TEST CASE 1
### Input
```bash
Enter Row & Col : 2 3
7 6 8
1 9 4
```
### Output
```bash
Matrix (2x3):
7 6 8
1 9 4
```
