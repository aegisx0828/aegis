Ref Document
=============
> ###### Markdown ref : https://gist.github.com/ihoneymon/652be052a0727ad59601#23-목록 , https://wikidocs.net/1678

Solr Project 
=============
* 공식 홈페이지 http://lucene.apache.org/solr/
* 위키 https://wiki.apache.org/solr/FrontPage
* 컨플루언스 https://cwiki.apache.org/confluence/display/solr/About+This+Guide

>1.solr 디렉토리 구조
=============
* http://dev-b.blogspot.kr/2012/10/apache-solr-3-enterprise-search-server.html


2.solrcloud 시 sqlconfig.xml 위치
=============
* 참고 사이트 : https://stackoverflow.com/questions/30093340/cannot-find-proper-solrconfig-xml-file-for-configuration-in-solr-5-1-0
*  ../solr-5.1.0/server/solr/configsets/data_driven_schema_configs **해당 위치에 존재함**
```xml
<dataConfig>
  <dataSource type="JdbcDataSource" 
              driver="com.mysql.jdbc.Driver"
              url="jdbc:mysql://localhost/dbname" 
              user="user-name" 
              password="password"/>
  <document>
    <entity name="id" 
            query="select id,name,desc from mytable">
    </entity>
  </document>
</dataConfig>
```

3.solr RDB 연동 참고
=============
* https://wiki.apache.org/solr/DataImportHandler

* oracle Driver 설치 필요 : server/lib 폴더에 jar 파일 설치 : http://www.oracle.com/technetwork/database/features/jdbc/index-091264.html

* solrcloud 버전으로 처음 진행하다가, solrconfig.xml 설정문제(zookeeper 확인필요)로 standalone 버전으로 진행
  1. solr 서버 기동
  2. core 생성 시 오류가 날 경우(Unable to create core Caused by: org.apache.solr.handler.dataimport.DataImportHandler)
  참조 : https://stackoverflow.com/questions/14827375/solr-4-1-dataimporthandler-classnotfoundexception
  3. solr core가 생성 될때, solrconfig.xml, data-config.xml 등 (../solr/configsets/data_driven_schema_configs/) 위치의 설정파일들이 core 디렉토리에 복사본이 만들어진다.
  
* solr rdb 연동 예제 : http://blog.naver.com/mankeys/220914286596

4.solr RDB 연동 인덱싱 방법 정리
=============
* 1. Solr 서버 설치
* 2. Solr 서버 start
* 3. Solr Core 생성
* 4. solrconfig.xml, data-config.xml, managed-schema 설정
* 5. Indexing 실행
> * 첫 설정 시 core를 생성하면 ../server/solr/configsets/data_driven_schema_configs/conf 안의 설정 내용들이 core의 설정으로 초기화 됨
> * uniqueKey 가 default로 id로 설정되어 있어 이부분을 example test로 empno 로 변경 함.
> * solrconfig.xml : data-config.xml 연동 설정 및 solr-dataimport lib 패스 추가 </p>
> * data-config.xml : 실제 db 연결정보 및 indexing 할 테이블/entity 정리 </p>
> * managed-schema : indexing 할 테이블 컬럼 type 및 uniqueKey 설정</p>

5.solr 서버에 arirang 환경 설치
=============
* 참조 : https://m.blog.naver.com/PostView.nhn?blogId=kgj1&logNo=220676136150&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F

