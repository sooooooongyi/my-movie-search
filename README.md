# 📝 My-Movie-Search

## 프로젝트 소개

영화검색 API를 이용해 영화를 검색할 수 있는 My-Movie-Search 서비스를 구현합니다.

## 기술 스택

- Vue
- JavaScript
- SaSS(SCSS)

## 프로젝트 결과

![ezgif com-gif-maker (5)](https://user-images.githubusercontent.com/69751205/136702717-d56db044-d83d-4d1d-a1d2-b0abb82938c3.gif)

## 배포

[배포](https://hardcore-roentgen-18a9a0.netlify.app)

## 프로젝트 설명

`페이지`

### Home

- '/' 로 접근 가능합니다.
- home과 likeList에 접근 가능한 네비게이션바가 있습니다.
- 입력창에 검색어를 입력하시면 MoviesPage로 넘어갑니다.

### MoviesPage

- 검색 결과를 무한 스크롤로 보여줍니다.
- 네비게이션과 재검색을 위한 입력창이 있습니다.
- 각 영화 카드를 클릭했을 때 MovieDetailPage로 이동합니다.

### MovieDetailPage

- 영화에 대한 상세 정보를 나타냅니다.

### likeMoviesPage

- 상세 페이지에서 Like 버튼이 클릭된 영화들을 볼 수 있습니다.

`data`

페이지들 사이에 계층적 관계가 명확하지 않아 Props가 아닌 Vuex로 필요한 모든 데이터를 fetch 하고 관리했습니다.

`추가기능`

- MovieDetailPage에 좋아요 버튼을 누르면 리스트에 담기도록 구현했습니다.
- F5를 눌러도 검색어, 검색 결과, 좋아요 리스트가 사라지지 않도록 구현했습니다.

`아쉬운점`

- 반응형 페이지를 만들지 못했습니다.
- 사용자 API 키를 .env에 입력해두고 process.env로 접근하려 했으나 `process is not defined`를 해결하지 못했습니다. 💦💦
