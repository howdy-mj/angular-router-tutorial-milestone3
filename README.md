# RouterTutorialMilestone3

해당 프로젝트는 Angular 공식문서 튜토리얼의 'SPA에 라우터 활용하기' > '라우터 튜토리얼: 히어로들의 여행' 마일스톤3의 '히어로 추가 기능' 까지 진행한 부분입니다.

기존 '튜토리얼: 히어로들의 여행'에서 가져왔으며, `styles.css`도 내용을 추가하였습니다.

- [(영문) Router tutorial: tour of heroes](https://angular.io/guide/router-tutorial-toh#milestone-3-heroes-feature)
- [(한글) 라우터 튜토리얼: 히어로들의 여행](https://angular.kr/guide/router-tutorial-toh#%EB%A7%88%EC%9D%BC%EC%8A%A4%ED%86%A4-3-%ED%9E%88%EC%96%B4%EB%A1%9C-%EA%B4%80%EB%A6%AC-%EB%AA%A8%EB%93%88)

`package.json`

```json
"dependencies": {
    "@angular/animations": "~11.2.7",
    "@angular/common": "~11.2.7",
    "@angular/compiler": "~11.2.7",
    "@angular/core": "~11.2.7",
    "@angular/forms": "~11.2.7",
    "@angular/platform-browser": "~11.2.7",
    "@angular/platform-browser-dynamic": "~11.2.7",
    "@angular/router": "~11.2.7",
    "rxjs": "~6.6.0",
    "tslib": "^2.0.0",
    "zone.js": "~0.11.3"
  },
  "devDependencies": {
    "@angular-devkit/build-angular": "~0.1102.6",
    "@angular/cli": "~11.2.6",
    "@angular/compiler-cli": "~11.2.7",
    "@types/jasmine": "~3.6.0",
    "@types/node": "^12.11.1",
    "codelyzer": "^6.0.0",
    "jasmine-core": "~3.6.0",
    "jasmine-spec-reporter": "~5.0.0",
    "karma": "~6.1.0",
    "karma-chrome-launcher": "~3.1.0",
    "karma-coverage": "~2.0.3",
    "karma-jasmine": "~4.0.0",
    "karma-jasmine-html-reporter": "^1.5.0",
    "protractor": "~7.0.0",
    "ts-node": "~8.3.0",
    "tslint": "~6.1.0",
    "typescript": "~4.1.5"
  }
```

## 프로젝트 열기

`프로젝트 실행하기`

```shell
# 설치
$ yarn
# or
$ npm install

# 실행
$ ng serve
# http://localhost:4200/ 에서 확인 가능
```

해당 프로젝트를 실행하면,

```
src/app/heroes/hero-list/hero-list.component.ts:12:14 - error NG6007: The Component 'HeroListComponent' is declared by more than one NgModule.
```

라는 에러가 뜨며, 이는 '라우터 튜토리얼: 히어로들의 여행'에서 '히어로 모듈 라우터 설정'부터 진행하시면 해결할 수 있습니다.

공식문서

- [(영어) Hero feature routing requirements](https://angular.io/guide/router-tutorial-toh#hero-feature-routing-requirements)
- [(한글) 히어로 모듈 라우터 설정](https://angular.kr/guide/router-tutorial-toh#%ED%9E%88%EC%96%B4%EB%A1%9C-%EB%AA%A8%EB%93%88-%EB%9D%BC%EC%9A%B0%ED%84%B0-%EC%84%A4%EC%A0%95)
