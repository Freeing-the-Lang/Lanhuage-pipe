# 🧩 Language-pipe
**다중 언어 파이프라인 실험 프로젝트**

---

## 📘 개요
Language-pipe는 여러 프로그래밍 언어를 **파이프처럼 연결**해,  
한 언어의 출력이 다른 언어의 입력이 되는 구조를 실험하는 프로젝트다.  
목표는 언어 간 경계를 최소화하고, **자연스럽게 흐르는 코드 체계**를 만드는 것이다.  

---

## ⚙️ 핵심 아이디어
- **Pipe Flow:** `Rust → C++ → ASM → ProofLedger`
- **중간 언어(C++)**는 각 언어의 구문 트리를 연결하는 **허브** 역할을 함
- **ProofLedger 통합:** 각 변환 단계의 해시를 기록해 **재현 가능한 빌드** 보장
- **Self-build Workflow:** GitHub Actions를 통한 자동 빌드 및 릴리즈

---

## 🧱 구조 (예시)
```
Lanhuage-pipe/
 ├── src/
 │    ├── parser_rust.rs
 │    ├── transpiler_cpp.cpp
 │    └── assembler_out.asm
 ├── proofledger.txt
 ├── LICENSE
 └── .github/workflows/
      └── build.yml
```

---

## 🧾 향후 계획
- 언어 간 타입 매핑 자동화 (`Rust struct ↔ C++ class ↔ ASM layout`)
- ProofLedger 자동 생성 및 서명 기능
- 파이프라인 GUI 시각화
- “Freeing-the-Lang” 프로젝트와의 연계

---

## 🪪 라이선스
MIT License © 2025
