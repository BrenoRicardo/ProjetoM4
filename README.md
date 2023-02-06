# ProjetoM4
# Perguntas respondidas no site
1a : 5 Jogos grátis mais avaliados
select name,(positive_ratings+negative_ratings)as avaliacoes,( (positive_ratings/ (positive_ratings+negative_ratings) )*100) as porcentagem_positiva, ( (negative_ratings/(positive_ratings+negative_ratings))*100)as porcentagem_negativa from steam where price = 0 order by avaliacoes desc limit 5 ;
2a : 5 jogos pagos mais avaliados 
select name,(positive_ratings+negative_ratings)as avaliacoes,( (positive_ratings/ (positive_ratings+negative_ratings) )*100) as porcentagem_positiva, ( (negative_ratings/(positive_ratings+negative_ratings))*100)as porcentagem_negativa from steam where price > 0 order by avaliacoes desc limit 5 ;
3a : 5 jogos mais avaliados por menos de 9 USS
select name,(positive_ratings+negative_ratings)as avaliacoes,( (positive_ratings/ (positive_ratings+negative_ratings) )*100) as porcentagem_positiva, ( (negative_ratings/(positive_ratings+negative_ratings))*100)as porcentagem_negativa from steam where price between 1 and 10 order by avaliacoes desc limit 5 ;
4a :	5 jogos mais avaliados 
select name,(positive_ratings+negative_ratings)as avaliacoes,( (positive_ratings/ (positive_ratings+negative_ratings) )*100) as porcentagem_positiva, ( (negative_ratings/(positive_ratings+negative_ratings))*100)as porcentagem_negativa from steam order by avaliacoes desc limit 5 ;
