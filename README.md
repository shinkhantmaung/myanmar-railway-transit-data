
# Myanmar Railway Transit Data - Simplify JSON

ပို့ဆောင်ရေးနှင့်ဆက်သွယ်ရေးဝန်ကြီးဌာန ၊ မြန်မာ့မီးရထားမှ ပြေးဆွဲနေသော မီးရထားခရီးစဉ်များအား စုစည်း၍ App များ Website များတွင် အသင့် အသုံးပြုနိုင်သော JSON Data အဖြစ် ပြောင်းလဲ ထားခြင်းဖြစ်သည်။

## TODOs

- [x] String များအား JSON ဖြစ်အောင် Parse လုပ်ထားရန်။
- [x] Whitespace အပိုများ ဖယ်ထုတ်သန့်စင်ထားရန်။
- [x] ရပ်နားသည့် ဘူတာများ ဖြည့်စွက်ပေးရန်။
- [x] လက်မှတ်နှုန်းထားများ ဖြည့်စွက်ပေးရန်။
- [ ] ရန်ကုန်မြို့ပတ် ခရီးစဉ်များ ဖြည့်စွက်ပေးရန်။
- [ ] မန္တလေးမြို့ပတ် ခရီးစဉ်များ ဖြည့်စွက်ပေးရန်။
- [ ] ဘူတာများ၏ geo lat long အချက်အလက်များ ဖြည့်စွက်ပေးရန်။

## List of files

 - `json/route-data-by-id.json` ခရီးစဉ်အလိုက် ရပ်တန့်ဘူတာများ ၊ ထွက်ခွာ နှင့် ဆိုက်ရောက်အချိန်များ ၊ လက်မှတ်နှုန်းထားများ ပါဝင်ပါသည်။

 - `json/station-data-by-id.json` သက်ဆိုင်ရာ ဘူတာများ၏ နာမည် ၊ lat long  အချက်အလက်များ ပါဝင်ပါသည်။

 - `json/train-data-by-id.json` ရထားခရီးစဥ် အမည် ၊ အမျိုးအစား နှင့် ပြေးဆွဲ နေ့ရက် အချက်အလက်များ ပါဝင်ပါသည်။

## APIs
## Get list of Stations
### Request

`GET /api/v1/stations`

    curl -i -H 'Accept: application/json' https://myanmar-railway-api.vercel.app/api/v1/stations

### Response

    HTTP/1.1 200 OK
    Date: Thu, 24 Feb 2011 12:36:30 GMT
    Status: 200 OK
    Connection: close
    Content-Type: application/json
    Content-Length: 2

    [
     {
      "id": "158",
      "name_en": "Kawt Che Station",
      "name_mm": " ကော့ချဲ ဘူတာ",
      "lat_long": null,
      "internal_notes": null
     }
    ]

 ## Get list of Trains
### Request

`GET /api/v1/trains`

    curl -i -H 'Accept: application/json' https://myanmar-railway-api.vercel.app/api/v1/trains

### Response

    HTTP/1.1 200 OK
    Date: Thu, 24 Feb 2011 12:36:30 GMT
    Status: 200 OK
    Connection: close
    Content-Type: application/json
    Content-Length: 2

    [
     {
      "id": "1",
      "name_mm": "အမှတ်(၁) အဆန်",
      "name2_mm": "ရန်ကုန် - မန္တလေး",
      "name_en": "1 UP",
      "name2_en": "Yangon - Mandalay",
      "display_order": 1,
      "type_price_mm": [
      null,
      null
      ],
      "type_price_en": [
      null,
      null
      ],
      "type_name": "စာပို့ရထား",
      "note": "ရက်ခြား"
      }
    ]

## Disclaimer
ဤအချက်အလက်များသည် ပို့ဆောင်ရေးနှင့်ဆက်သွယ်ရေးဝန်ကြီးဌာန ၊ မြန်မာ့မီးရထားမှ တရားဝင် စီမံထိမ်းသိမ်း၍ ဖြန့်ဖြူးထားခြင်း <b>မဟုတ်ပါ</b>။ အချက်အလက် တိကျမှုအားလည်ကောင်း၊ ပြည့်စုံမှုအားလည်ကောင်း အာမမခံပါ။


## License
ဤအချက်အလက်များအား CC BY SA 4.0 ပါ ခွင့်ပြုချက်နှင့်အညီ ပြင်ဆင်၍ ပြန်လည်ဖြန့်ဝေသည်။ ဤအချက်အလက်များအား CC BY SA 4.0 ပါ ခွင့်ပြုချက်များ၊ ကန့်သန့်ချက်များနှင့်အညီ ရယူခြင်း၊ ပြင်ဆင်ခြင်း၊ ဖြန့်ဝေခြင်းများ ပြုလုပ်နိုင်သည်။
