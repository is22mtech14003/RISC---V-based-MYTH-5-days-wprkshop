# RISC-V-based-MYTH 5 days wprkshop
# Day 1
[RISC-V](https://www.synopsys.com/glossary/what-is-risc-v.html#:~:text=What%20are%20the%20benefits%20of,facilitating%20faster%20time%20to%20market.)
## How ro RISC V work on our computer and flow of working
suppose you writen a code in C language, that code could be like sawping and any other and you want to run this code on your machine then how will run. so first compiller convert this code into assembly language, and again assembler convert this code into machine level language (it means zero and one form and then impliment on hardware) and after that show the result 
## So what the role of RISC V architecture
RISC V architecture tell the how c language code will convert into instruction set and its defined whole procsss of execution
![2](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/739397e4-defe-4da9-9268-b8f534f58e43)
![risk1](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/8835cd9b-48c5-4fbc-b8a6-126c27f1b3ba)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/dbc64531-3f18-40dd-a037-7e3852ec2ae0)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/c74f3c01-bf0c-474d-a184-ca1a75f45e33)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/498299ee-7a3d-48fd-a4d5-d8751d551a2d)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/f7829d4b-6dcf-452e-85ef-82a3e913b3e0)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/d8ea4cbe-2acc-455b-9d8d-714b46911d50)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/1e23819d-fa2b-40e8-9f5f-9759d1ffa22c)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/b0c65a65-f212-4457-a6e3-5654baccadb2)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/a4b895eb-42c6-41ee-8689-c7b5135fbd16)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/0e1e6382-55f6-4e67-b9c7-0802b0e10f09)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/74d72ef1-cc4a-4eec-b4bb-7bdd4a758eec)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/14b2d24e-413c-4faf-8fe7-1231118db91c)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/6832477a-d07a-4d4f-8c63-f444baa1fe57)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/d5a1094e-7b66-4740-ba95-fa272e044cc8)

# Day 2

# Aplication binary interface and basic verification flow

On This day, we devloped deep into the lower layers on how the higher layer instructions in c are translated to machine understandable codes. Just like how application program interface (API) is used by application programs to access the standard libraries, an application binary interface or system call interface is utilised hardware resources . The ISA is inherently divided into two parts: User & System ISA and User ISA the latter is available to the user directly by system calls.
### Now, how does the ABI access the hardware resources?
- It uses different registers(32 in number) which are each of width XLEN = 32 bit for RV32 (~XLEN = 64 for RV64) . On a higher level of abstraction these registers are accessed by their respective ABI names.

For base integer instructions there are broadly 3 types of of such registers:
- I-type : For instructions having immediate values as operands.
- R-type : For instructions having only registers as operands.
- S-type : For instructions used for storing operations.


![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/50f7c3e9-6763-4190-84bb-aa34bba4ca6e)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/8c11a442-f4f0-4762-8a8f-6e444315166a)

![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/4b2c7366-2fa7-4653-8c1f-40c35d3ddd48)
![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/2a540952-6328-4bb6-9102-3a671f6c4112)

![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/0ff682c2-c236-43a6-aa2d-03b0f3913f74)


|:---:|:---:|
|![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/c4620dcc-f73c-4497-a13c-108afc586378)|![image](https://github.com/is22mtech14003/RISC---V-based-MYTH-5-days-wprkshop/assets/120499567/5eb3cc2c-b7ad-4812-af79-4b508c9971ea)|


