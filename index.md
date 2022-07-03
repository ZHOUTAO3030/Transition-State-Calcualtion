---
Title: Transition State Calculation
## Steps of searching complex transition state  

1. Structure Optimization of initial strcuture and final structure
2. Search optimal input with Cl-NEB methods
3. Dimer calculation for accurate transition state
4. Data visulization

## 1. Omit
## 2.Cl-NEB Methods
### 2.1 Generate intermediate images

'dist.py' can be used to find similarity of initial structure and final strcutre. Here disy.py calculates distance summation of  all the corresponding atoms. The output will be smaller than 5 Å. Remember to check whether the numbering is one-to-one correspondence bewteen intital state and final state.

>dist.pl POSCARis POSCARfs
>7.91680185884989


' idpp.py ' will be used for generate 4 images. The nuber of images can be approximated by value od dist.pl/0.8.The prequistes is that the system supports PYMATGEN.

>module load anaconda3\
>conda activate pymatgen\
>python3 idpp.py POSCARis POSCARfs 4

>00 01 02 03 04 05 

> nebmovie.pl 0 #0 represents xyx file is generated from POSCAR. 1 represents CONTCAR. 







A transition structure is the molecular configuration that separates reactants and products. This page records the whole process of searching transition state of Cyclohexane Dehydrogenation on Pt-graphene, combining btoh Cl-NEB and dimer methods.


## Cl-NEB
![Example](https://user-images.githubusercontent.com/108607220/177032214-5ac790ed-91ab-4c26-a589-00fa08188ad9.png)

## Dimer
![image](https://user-images.githubusercontent.com/108607220/177032398-5cf282e6-3dbf-47a5-a106-2fd3ded0cbb1.png)
![image](https://user-images.githubusercontent.com/108607220/177036726-78575112-5111-439a-9b2d-c3b6273754b7.png)
## Cyclohexane Dehydrogenation on Pt-graphene
## Initializing NEB Calculations
### Linear interpolation VS Image Dependent Pair Potential
## Frequency Calculation






Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![https://user-images.githubusercontent.com/108607220/177031871-b05cf872-ffa9-439b-b940-353fa1d48da6.png]
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/ZHOUTAO3030/Transition-State-Calcualtion/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
