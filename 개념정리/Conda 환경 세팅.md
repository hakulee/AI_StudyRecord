1. Conda 기본 명령어:
   - 가상 환경 생성
     ```bash
     conda create --name myenv python=3.9
     ```
     
   - 가상 환경 활성화
     ```bash
     conda activate myenv
     ```
     
   - 가상환경 비활성화
     ```bash
     conda deactivate
     ```
     
   - 가상환경 리스트 확인
     ```bash
     conda env list
     ```
     
   - 패키지 설치
     ```bash
     conda install numpy // pip install numpy 
     ```

    - 원하는 버전의 패키지 설치
      ```bash
      pip install numpy==x.y.z
      ```
        
   - 패키지 업데이트
     ```bash
     conda update numpy
     ```

   - 패키지 제거
     ```bash
     conda remove numpy
     ```

   - 가상 환경 내보내기 (YAML/TXT 파일 생성)
     ```bash
     conda env export > environment.yml
     # Conda 환경을 재현하려면 conda env export > environment.yml 명령어를 사용하는 것이 더 적합
     
     pip freeze > requirements.txt
     # 이 방법은 pip로 설치된 패키지 목록만 저장하므로,
     conda 환경에서 설치된 conda 패키지나 시스템 의존성 등은 반영되지 않습니다.
     ```

   - 가상 환경 적용하기
     ```bash
     conda env create -f environment.yml -n new_env_name

     pip install -r requirements.txt
     ```

   - 가상환경 삭제
     ```bash
     conda remove --name myenv --all
     ```
  
