MATCH (p:Persona)-[:AMIGO_DE]-(amigo:Persona)
WHERE p.ciudad <> amigo.ciudad
RETURN DISTINCT p.nombre