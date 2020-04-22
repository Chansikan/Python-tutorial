
연구제목
코로나바이러스-19 감염환자의 인구사회학적 및 의학적 특성을 분석하여 예후를 예측하는 기계학습 알고리듬의 개발 및 검증
Machine learning for predicting prognosis in COVID-19 patients based on sociodemographic and medical characteristics in South Korea 
연구참가자
 원내: 안찬식, 임현선, 장정현, 최윤정, 김성우
 원외: 김동욱
연구목적
의료 서비스 이용 패턴에 근거하여 1년 이내 뇌졸중을 진단받을 가능성을 예측하는 인공지능 알고리듬을 개발하고 검증
연구내용
및 대상
2020년 3월까지 대한민국에서 신종 코로나바이스러스로 확진된 환자들을 대상으로 한다. 인구사회학적 정보, 기저질환, 투약내역, 감염경로 등, 예후와 관련이 있을 수 있다고 생각되는 요인들을 포함하는 국민건강보험공단의 맞춤형 자료를 이용한다. 
연구방법
다양한 요인들 중 예후(사망 여부 및 인공호흡기 혹은 체외막산소화장치가 필요하였는지 여부 등) 유의한 관련성을 보인 요인들을 조사하고, 이러한 요인을 이용하여 예후를 예측할 수 있는 인공지능 알고리듬을 개발하고 검증한다.
연구결과 
기대효과
성공적인 예후 예측모델이 만들어진다면, 신종 코로나바이러스 감염병 진단 후 예후를 미리 가늠할 수 있어 더 적절한 진료와 효율적인 의료자원 이용을 도모할 수 있다.


국민건강보험공단의 자료에서 얻을 수 있는 정보들 중, 코로나바이러스-19 감염환자의 예후와 관련성이 있을 수 있다고 생각되는 요인들을 분석하고 정하는 작업을 한다. 
- 인구사회학적 요인: 나이, 성별, 국적, 거주지, 경제적 상황, 장애 유무 및 중증도, 독거 여부, 발병원인, 감염경로
- 의학적 요인: 증상 유무, 흡연 여부, 음주 여부 및 정도, 건강검진 수진 여부 및 결과, 동반 상병, 투약 정보

이렇게 정해진 변수들과 예후 평가 인자들에 대한 정보가 포함되도록 하여, 코로나바이러스-19 감염환자의 국민건강보험공단 맞춤형 자료를 신청한다.

조사한 요인들의 기술적 통계 결과를 정리한다. 진단 후 예후에 따라 환자군을 나누고, 각 군에서 이 요인들의 분포 및 대표값에 유의한 차이가 있는 지 조사한다.

진단 후 예후와 유의한 연관성을 보이는 인자들을 찾고, 그 관련성의 크기를 다양한 방법으로 측정한다: odds ratio, variable importance, permutation feature importance, mutual information, etc.
또한, 다양한 상황과 방법에서 일관되게 유의하고 의미있는 크기의 연관성을 보이는 인자는 무엇인지 조사한다.

환자군을 예후인자의 분포를 균질하게 하여 7:3으로 training:test 군으로 나눈다. Training 군에서, 다양한 feature selection 방법, machine learning classifier (logistic regression with regularization, support vector machine, linear discriminant analysis, random forest, adaptive boosting, multiple layer perceptron, etc), hyperparameter 조합들 중 가장 일반화가 잘 되는 모델을 찾는다. 이를 위해서는 cross validation을 시행한다. 이렇게 학습된 모델을 test 군에서 최종 테스트하여 모델의 정확도를 평가한다.








