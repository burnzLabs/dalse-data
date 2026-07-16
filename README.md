# dalse-data

달세(Dalse) 앱이 사용하는 데이터를 제공합니다.

| 경로 | 내용 |
|---|---|
| `exchange/krw-rates.json` | KRW 기준 환율 |
| `exchange/meta.json` | 환율 갱신 시각 |
| `holidays/kr.json` | 한국 공휴일 |
| `presets/kr-subscription.json` | 구독 서비스 프리셋 |

## 형식

**환율** — `unit`의 `(100)` 접미사는 100단위 가격을 뜻합니다.

```json
{ "unit": "USD", "name": "미국 달러", "englishName": "US Dollar", "price": "1493", "symbol": "$", "symbolBeforeAmount": true, "useDecimal": true }
```

**공휴일**

```json
{ "date": "2026-01-01", "names": ["신정"] }
```

**프리셋**

```json
{ "id": "preset-netflix", "name": "Netflix", "category": "영상 스트리밍", "amount": 17000, "currency": "KRW", "billing_cycle": "monthly", "icon": "tv", "color": "#E50914" }
```
