EXERCISE 4
-- 1. List all directors of Pixar movies (alphabetically), without duplicates
SELECT DISTINCT director FROM movies
WHERE studio = 'Pixar'
ORDER BY director ASC;

-- 2. List the last four Pixar movies released (most recent to least)
SELECT * FROM movies
WHERE studio = 'Pixar'
ORDER BY year DESC
LIMIT 4;

-- 3. List the first five Pixar movies sorted alphabetically
SELECT * FROM movies
WHERE studio = 'Pixar'
ORDER BY title ASC
LIMIT 5;

-- 4. List the next five Pixar movies sorted alphabetically
SELECT * FROM movies
WHERE studio = 'Pixar'
ORDER BY title ASC
LIMIT 5 OFFSET 5;
