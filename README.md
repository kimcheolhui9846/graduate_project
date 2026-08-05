# ⚠ 이 저장소는 통합되었습니다

이 저장소의 노트북들은 **2026-08-05에 아래 저장소로 병합**되었습니다.

### → https://github.com/kimcheolhui9846/fashion-recommendation

병합 위치: [`notebooks/`](https://github.com/kimcheolhui9846/fashion-recommendation/tree/main/notebooks)

**커밋 이력까지 함께 옮겼으므로** 여기서 볼 수 있는 것은 전부 그쪽에도 있습니다.
앞으로의 작업은 통합 저장소에서 진행합니다.

---

## 왜 통합했나

이 저장소에는 **크롤링 → 분류 실험 → 데이터 문제 규명**까지의 기록이,
다른 저장소에는 **재설계된 파이프라인**이 있어 서사가 끊겨 있었습니다.

최종 결과만 보면 *"왜 분류를 쓰지 않는가"* 에 답할 수 없습니다.
분류를 포기한 근거가 이 저장소에 있기 때문입니다.

```
[이 저장소]  크롤링 → 노이즈 제거 → CMT 실험 → ConvNeXt v1 (88.23%)
                    ↓
             "88%가 진짜인가?" → pHash 누수 검사 → 중복 라벨 진단
                    ↓
[통합 저장소] 카테고리 병합 → 검출 + 임베딩 검색으로 재설계 → 파인튜닝
```

## 병합된 노트북

| 원래 이름 | 통합 후 |
|---|---|
| `Untitled-2.ipynb` | `notebooks/01_크롤링_상품수집.ipynb` |
| `크롤링(노이즈제거모델)-1.ipynb` | `notebooks/02_노이즈제거_YOLO.ipynb` |
| `데이터 정제 파이프라인.ipynb` | `notebooks/03_데이터정제_파이프라인.ipynb` |
| `cmt 모델.ipynb` | `notebooks/04_CMT_분류실험.ipynb` |
| `conv.ipynb` | `notebooks/05_ConvNeXt_누수검사.ipynb` |
| `33.ipynb` | `notebooks/06_중복라벨_시각진단.ipynb` |

`Untitled-1.ipynb`와 `Untitled-2_backup.ipynb`는 `Untitled-2.ipynb`와
**내용이 완전히 동일**해(해시 일치) 통합 시 하나만 남겼습니다.
