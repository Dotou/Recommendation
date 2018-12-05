Time and Location Aware Points of Interest Recommendation in Location-Based Social Networks 
《JOURNAL OF COMPUTER SCIENCE AND TECHNOLOGY》2018
====
issue：
----
Current studies on representation learning for POI recommendation embed both users and POIs in a common latent space,and users’ preference is inferred based on the distance/similarity between a user and a POI. Such an approach is not in accordance with the semantics of users and POIs as they are inherently different objects.

TransTL：
-----
models the spatial and temporal information as a relationship connecting users and POIs
- the embedding of a <time, location> pair corresponds to a translation from embeddings of users to POIs. Since the POI embedding should
be close to the user embedding plus the relationship vector (TransR)
-the recommendation can be performed by selecting the top-k POIs similar to the translated POI, which are all of the same type of objects.

datasets:
------
Location-based social networks(LBSN) datasets: Foursquare and Gowalla
----

1、POIs推荐应考虑时间和空间两方面影响，TransREC依据序列推测下一个item，为basket rec;
2、GE，STELLAR和Geo-Teaser在同一潜在空间下学习的用户与POIs向量，不能表示用户与POIs的本质，用户和POIs是不同的主体
3、在<时间t，地点l>关系下，用户的POIs并不相同，例如，用户A在午饭时在校园POIs为食堂，在午饭时在商场POIs为餐厅，用户的通过TransR在不同的关系空间下学习用户，POIs向量
4、加入POI-POI关系，缓解冷启动问题
