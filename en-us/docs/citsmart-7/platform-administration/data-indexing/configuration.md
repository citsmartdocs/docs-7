Title: Managing content indexing

# Managing Content Indexing

CITSmart uses Apache SOLR to index content created in the Knowledge Management and makes it available in the Knowledge Portal search system.

## What to do before

In order for Knowledge Indexing to work correctly, it is necessary:

* [x] Install the Apache SOLR component as shown in the [installation manual][1].

## Parametrizing the indexing service

1. Access the main menu Parametrization > CITSmart Parameters;
2. Configure parameter 304 by entering the URL of the SOLR component;

    ```sh
    http://localhost:8983/solr/collection_name
    ```

3. Configure parameter 308 stating the number of items to be indexed each time;
4. Configure parameter 332 stating whether synchronization with the Indexing server is active;
5. Access the main menu System > Settings > Knowledge Management (Indexing) and click on "Update the index server".

## Managing content

1. Access the main menu System > Settings > Kowledge Management (Indexing);
2. To index the available knowledge, click on "Index Knowledge Base", or to remove the knowledge already indexed, click on "Remove 
Knowledge Base Indexing".


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>06/25/2019

[1]:/en-us/citsmart-7/get-started/installation-and-upgrade/download-software.html#servidor-de-indexacao-apache-solr_1
