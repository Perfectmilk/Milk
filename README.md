//
//  main.m
//  作业_2
//
//  Created by 李广鹏 on 15/7/30.
//  Copyright (c) 2015年 李广鹏. All rights reserved.
//

#import <Foundation/Foundation.h>

int main(int argc, const char * argv[]) {
    
#pragma mark -第一次
//    int number[20],max = 0;
//    for (int i = 0; i < 20; i ++) {
//        number[i] = arc4random()%91 + 10;
//        if (number[i] > max) {
//            max = number[i];
//        }
//        printf("%d\t",number[i]);
//    }
//    printf("\n最大的为%d",max);
    
#pragma mark -第二次
//    int count = 0;
//    for (int a = 1; a < 10; a ++) {
//        for (int b = 1; b < 10; b ++) {
//            for (int c = 1; c < 10; c++) {
//                if ((a*a*a+b*b*b+c*c*c) == (a*100 + b*10 +c)) {
//                    printf("\n%d\t",a*100 + b*10 +c);
//                    count ++;
//                }
//            }
//        }
//    }
//    printf("\n共有%d个花仙数",count);
    
    
#pragma mark -第三次
//
//    for (int a = 0; a < 10; a ++) {
//        for (int b = 0; b < 10; b++) {
//            for (int c = 0; c < 10; c++) {
//                if ((a*100 + b*10 + c) + (c*100 + b*10 +a) == 1333) {
//                    printf("a = %d   b = %d   c = %d\n",a,b,c);
//                }
//            }
//        }
//    }
    
#pragma  mark -第四次
    
    int year,month,day;
    int p = 1;
    while (p) {
    printf("\n请输入您的生日，如1991-01-01:");
    scanf("%d-%d-%d",&year,&month,&day);
    switch (month) {
        case 1:
        case 3:
        case 5:
        case 7:
        case 8:
        case 10:
        case 12:
            if (day > 31 || day < 1) {
                printf("您的日期输入有误,请重新输入");
            }
            else{
                p = 0;
            }
            break;
        case 4:
        case 6:
        case 9:
        case 11:
            if (day > 30 || day < 1) {
                printf("您的日期输入有误，请重新输入");
            }
            else{
                p = 0;
            }
            break;
        case 2:
            if (day > 29 || day < 1) {
                printf("您的日期输入有误，请重新输入");
            }
            else {
                p = 0;
            }
            break;

        default:
            printf("您的月份输入有误，请重新输入");
            break;
    }
    }
    printf("输入正确!");
    
    return 0;
}

