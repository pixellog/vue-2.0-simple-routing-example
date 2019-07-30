<template>
    <div>
        <header class="navbar navbar-expand-lg navbar-dark bg-primary">
            <a class="navbar-brand" href="/"><span class="sr-only">CODEF 개발가이드</span></a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">

                <div class="container">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <v-link class="nav-link" href="/docs">Documentation</v-link>
                        </li>
                        <li class="nav-item">
                            <v-link class="nav-link" href="/api">API Versioning</v-link>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="ml-auto form-inline text-light">

                <div class="input-group">
                    <input type="search" class="form-control text-light" placeholder="Search" aria-label="Search">
                    <div class="input-group-append">
                        <button type="submit" class="btn btn-sm btn-info">검색</button>
                    </div>
                </div>


                <select name="" id="" class="form-control text-light ml-3">
                    <option value="">Node.js</option>
                    <option value="">Java</option>
                    <option value="">PHP</option>
                    <option value="">Ruby</option>
                    <option value="">Python</option>
                </select>
                <span class="ml-3"><span class="text-info">최동철</span>님</span>
                <!--<button type="button" class="btn">로그인</button>-->
                <a href="#none" class="btn btn-outline-light btn-sm ml-3">로그아웃</a>
            </div>
        </header>

        <b-row class="no-gutters">
            <b-col cols="2">
                <b-navbar v-b-scrollspy:scrollspy-nested class="sidebar">
                    <b-nav pills class="flex-column">
                        <li class="nav-item"><v-link class="nav-link" href="/docs">개요</v-link></li>
                        <!--<b-nav-item href="/docs#item-1">개요</b-nav-item>-->
                        <b-nav pills class="flex-column">
                            <b-nav-item href="/docs#item-1-1">CODEF Architecture</b-nav-item>
                            <b-nav-item href="/docs#item-1-2">CODEF API Data</b-nav-item>
                            <b-nav pills class="flex-column">
                                <b-nav-item href="#item-1-2-1">Item 1-2-1</b-nav-item>
                                <b-nav-item href="#item-1-2-2">Item 1-2-2</b-nav-item>
                            </b-nav>
                        </b-nav>
                        <li class="nav-item"><v-link class="nav-link" href="/docs/dic">용어사전</v-link></li>
                        <li class="nav-item"><v-link class="nav-link" href="/docs/cert">인증방식</v-link></li>
                        <!--<v-link class="nav-link" href="/docs/dic">Documentation</v-link>-->
                        <!--<b-nav-item href="/docs/cert">인증방식</b-nav-item>-->
                        <b-nav pills class="flex-column">
                            <b-nav-item href="#item-3-1">Item 3-1</b-nav-item>
                            <b-nav-item href="#item-3-2">Item 3-2</b-nav-item>
                        </b-nav>
                        <b-nav-item href="/docs/prodoucts">상품</b-nav-item>
                        <b-nav-item href="/docs/errors">오류</b-nav-item>
                        <b-nav-item href="/docs/sandbox">샌드박스</b-nav-item>
                    </b-nav>
                </b-navbar>
            </b-col>

            <b-col cols class="border-left border-right">
                <div id="scrollspy-nested" style="position:relative; height:80vh; overflow-y:auto">
                    <div class="location">
                        <h2>보유계좌</h2>
                        <span>홈 > Documentation > 개요</span>
                    </div>
                    <div class="content">
                        <slot></slot>
                    </div>
                    <div class="update">업데이트: 2019-07-01</div>
                </div>
            </b-col>
            <b-col cols="3">
            </b-col>
        </b-row>

        <footer class="footer">
            <div class="row">
                <div class="col-md-6">
                    <a class="navbar-brand" href="/"><span class="sr-only">CODEF 개발가이드</span></a>
                    <div class="ml-md-5 mt-2">
                        <address class="m-0">서울특별시 영등포구 문래북로 116 (문래동 3가, 트리플렉스) 804호</address>
                        <p>사업자등록번호 113-86-32627 | 통신판매업 신고 2009-서울강남-00250 <br> © Heenam Co., Ltd. All right reserved.</p>
                    </div>
                </div>
                <div class="col-md row">
                    <ul class="list-unstyled col">
                        <li><a href="/about-us/about">회사소개</a></li>
                        <li><a href="/about-us/team">구성원소개</a></li>
                        <li><a href="/about-us/careers">채용</a></li>
                        <li><a href="/blog">기술블로그</a></li>
                    </ul>
                    <ul class="list-unstyled col">
                        <li><a href="/contact">서비스문의</a></li>
                        <li><a href="/legal/terms">이용약관</a></li>
                        <li><a href="/legal/privacy">개인정보취급방침</a></li>
                        <li><a href="/legal/email">이메일무단수집거부</a></li>
                    </ul>
                    <ul class="list-unstyled col">
                        <li><a target="_blank" href="">CODEF 공식 페이스북</a></li>
                        <li><a target="_blank" href="//www.heenam.co.kr">희남</a></li>
                        <li><a target="_blank" href="//www.espider.co.kr">이스파이더</a></li>
                        <li><a target="_blank" href="//www.daylifg.com">데일리금융그룹</a></li>
                    </ul>
                </div>
            </div>
        </footer>

    </div>
</template>

<script>
    import VLink from '../components/VLink.vue'

    export default {
        components: {
            VLink
        }
    }
</script>
