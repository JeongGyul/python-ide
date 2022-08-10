# python-ide
2022 8월 인공지능 부트캠프

파이썬을 위한 다양한 개발환경

## 수업 자료 내려받기
` $ git clone https://github.com/ai7dnn/python-ide.git `  

## 가상환경 생성(venv 활용)
 ` > python -m venv jnum `   
 ` > jnum\scripts\activate `  
 ` > pip install numpy jupyter `  
 ` > pip show numpy jupyter `  
 ` > deactivate `

## 가상환경 생성(conda 활용)
 ` > conda create -n cjmat matplotlib jupyter `   
 ` > conda activate cjmat `  
 ` > conda install pandas tensorflow `  
 ` > conda list pandas `
     > list: 하나의 패키지만 확인 가능  
 ` > conda list jupyter `  
 ` > conda deactivate `  
 
## 주피터 커널 생성
 ` > jupyter kernelspec list`  
 - 다음 명령은 반드시 생성된 가상환경을 활성화한 상태에서   
 ` > python -m ipykernel install --user --name jnum --display-name "py numpy"`  
   1. jnum: 커널이름
   2. 주피터에서의 표시이름: "py numpy"  
 
 ` > jupyter kernelspec list`  
 ` > jupyter notebook`  

## 현재 파이썬 확인 방법
 ` import site `  
 ` site.getsitepackages() `  
 
## 주피터 커널 삭제
 ` > jupyter kernelspec uninstall jnum `

