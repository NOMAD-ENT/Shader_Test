# Shader Test

본 저장소는 **NOMAD-ENT** 내부 테스트를 위해 제작된 **바디 전용(Body‑Only) 쉐이더** 샘플 모음입니다.  
저장소에 포함된 파일만으로는 완벽한 쉐이더 구동을 보장하지 못하며
일부 최적화 및 커스터마이징하여 사용해야 합니다.

## 폴더 구조

```text
Shader_Test/
├─ Map/                        # 테스트용 레벨 파일
└─ Shader/
    ├─ Materials/              
    │   ├─ CurveAtlas/         # 쉐이더 관련 커브 아틀라스
    │   └─ Master_Shader/      # 바디 관련 쉐이더 머트리얼
    └─ Textures/               # toon 관련 텍스쳐
```

## 사용 방법

1. **클론 또는 압축 해제**
   ```bash
   git clone https://github.com/NOMAD-ENT/Shader_Test.git
   ```
2. **셈플 메트리얼 사용**
   1. 언리얼 에디터에서 **`Map/TestMap.umap`** 을 열어 테스트 레벨을 로드합니다.
   2. 해당 레벨에는 **`Toon_Body`** 와 **`Toon_Hair`** 쉐이더를 적용한 각각의 Cube 및 Sphere 물체가 존재합니다.
   3. 추가적인 쉐이더 확인은 **`Shader/Materials/Master_Shader`** 디렉토리를 참고하세요.

> **중요:** 제공되는 파일은 Avatar 에 적용되는 쉐이더 프로젝트 소스를 일부 클론 한 것으로, 완벽히 작동 되지 않습니다.
