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
  
 - 생성된 가상환경을 활성화한 상태에서 kernelspec list 에서 보이는 python3
     * 가상환경의 kernel 임
 
 ` > jupyter kernelspec list`  
 ` > jupyter notebook`  

## 현재 파이썬 확인 방법
 ` import site `  
 ` site.getsitepackages() `  
 
## 주피터 커널 삭제
 ` > jupyter kernelspec uninstall jnum `
 
## 주피터 커널 생성 실습
- 주피터 커널 확인
 ` > jupyter kernelspec list`  

- 가상환경 jnp 생성과 커널 등록  
 ` > conda create -n jnp numpy jupyter `  
 ` > conda activate jnp `  
 ` > python -m ipykernel install --user --name jnp --display-name jnp `  
 ` > jupyter kernelspec list`  
 ` > conda deactivate `  

- 가상환경 jpd 생성과 커널 등록  
 ` > conda create -n jpd pandas jupyter `  
 ` > conda activate jpd `  
 ` > python -m ipykernel install --user --name jpd --display-name jpd `  
 ` > jupyter kernelspec list`  
 ` > conda deactivate `  
 
- 주피터 총 커널 확인  
 ` > jupyter kernelspec list `    
 
- 주피터 싱행해 각 커널 별로 확인 확인  
 ` > jupyter notebook `  
