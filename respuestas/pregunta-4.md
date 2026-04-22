MATCH (p:Persona)-[:AMIGO_DE]->(a:Persona) 
WITH p, count(a) AS total_amigos 
WHERE total_amigos > 1 
RETURN p.nombre, total_amigos