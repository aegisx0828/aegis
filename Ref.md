Ref Document
=============
> ###### Markdown ref : https://gist.github.com/ihoneymon/652be052a0727ad59601#23-목록 , https://wikidocs.net/1678

Solr Project 
-------------
* 공식 홈페이지 http://lucene.apache.org/solr/
* 위키 https://wiki.apache.org/solr/FrontPage
* 컨플루언스 https://cwiki.apache.org/confluence/display/solr/About+This+Guide
1. solr 디렉토리 구조
> http://dev-b.blogspot.kr/2012/10/apache-solr-3-enterprise-search-server.html

2. solrcloud 시 sqlconfig.xml 위치
> 참고 사이트 : https://stackoverflow.com/questions/30093340/cannot-find-proper-solrconfig-xml-file-for-configuration-in-solr-5-1-0

> ../solr-5.1.0/server/solr/configsets/data_driven_schema_configs **해당 위치에 존재함**
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
3. solr RDB 연동 참고
> https://wiki.apache.org/solr/DataImportHandler
> oracle Driver 설치 필요 : server/lib 폴더에 jar 파일 설치
