# signature-seach-Tool
signature seach Tool


## 요구 사항 정의
* Header detection: python으로 구현 
* Body, footer detection:yara 사용
* Header 탐지 후 Body와 Footer를 탐지하도록 구현한다.
* Signature rule은 json 형식으로 작성
* Signature rule을 메모리로 읽어들일 때 Tree 구조를 형성하도록 한다. 

## JSON file specification
```
  [
    {
      ""type": /* file type:string, ex) "jpeg/jfif" */,
      "extension": /* file extention:string, ex) "jpg" */,
      "offset": /* start position:integer, ex) 0 */,
      "signature": /* signature: hexadecimal string, ex) "FF D8 FF E0 xx xx 4A 46 49 46" */
     },
     ...
  ]
```
