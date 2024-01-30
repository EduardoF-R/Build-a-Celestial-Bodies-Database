--
-- PostgreSQL database dump
--

-- Dumped from database version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)
-- Dumped by pg_dump version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE universe;
--
-- Name: universe; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE universe WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE universe OWNER TO freecodecamp;

\connect universe

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: alien_life; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.alien_life (
    alien_life_id integer NOT NULL,
    name character varying(20) NOT NULL,
    civilization_age integer NOT NULL
);


ALTER TABLE public.alien_life OWNER TO freecodecamp;

--
-- Name: alien_life_alien_life_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.alien_life_alien_life_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.alien_life_alien_life_id_seq OWNER TO freecodecamp;

--
-- Name: alien_life_alien_life_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.alien_life_alien_life_id_seq OWNED BY public.alien_life.alien_life_id;


--
-- Name: galaxy; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.galaxy (
    galaxy_id integer NOT NULL,
    name character varying(20) NOT NULL,
    star_quantity integer,
    galaxy_age numeric(4,2),
    description text
);


ALTER TABLE public.galaxy OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.galaxy_galaxy_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.galaxy_galaxy_id_seq OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.galaxy_galaxy_id_seq OWNED BY public.galaxy.galaxy_id;


--
-- Name: moon; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.moon (
    moon_id integer NOT NULL,
    name character varying(20) NOT NULL,
    planet_id integer,
    is_spherical boolean,
    description text
);


ALTER TABLE public.moon OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.moon_moon_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.moon_moon_id_seq OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.moon_moon_id_seq OWNED BY public.moon.moon_id;


--
-- Name: planet; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.planet (
    planet_id integer NOT NULL,
    name character varying(20) NOT NULL,
    has_life boolean,
    is_a_planet boolean,
    star_id integer
);


ALTER TABLE public.planet OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.planet_planet_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.planet_planet_id_seq OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.planet_planet_id_seq OWNED BY public.planet.planet_id;


--
-- Name: star; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.star (
    star_id integer NOT NULL,
    name character varying(20) NOT NULL,
    star_age integer,
    galaxy_id integer,
    description text
);


ALTER TABLE public.star OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.star_star_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.star_star_id_seq OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.star_star_id_seq OWNED BY public.star.star_id;


--
-- Name: alien_life alien_life_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.alien_life ALTER COLUMN alien_life_id SET DEFAULT nextval('public.alien_life_alien_life_id_seq'::regclass);


--
-- Name: galaxy galaxy_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy ALTER COLUMN galaxy_id SET DEFAULT nextval('public.galaxy_galaxy_id_seq'::regclass);


--
-- Name: moon moon_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon ALTER COLUMN moon_id SET DEFAULT nextval('public.moon_moon_id_seq'::regclass);


--
-- Name: planet planet_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet ALTER COLUMN planet_id SET DEFAULT nextval('public.planet_planet_id_seq'::regclass);


--
-- Name: star star_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star ALTER COLUMN star_id SET DEFAULT nextval('public.star_star_id_seq'::regclass);


--
-- Data for Name: alien_life; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.alien_life VALUES (1, 'Xylophorian Envoys', 100000);
INSERT INTO public.alien_life VALUES (2, 'Zenthralis Seekers', 200000);
INSERT INTO public.alien_life VALUES (3, 'Quadrion Symbiotes', 300000);


--
-- Data for Name: galaxy; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.galaxy VALUES (1, 'milky_way', 100, 13.60, 'The galaxy containing the Sun and its Solar System, and therefore Earth.');
INSERT INTO public.galaxy VALUES (2, 'andromeda', 120, 14.00, 'Andromeda is the closest big galaxy to the Milky Way and is expected to collide with the Milky Way around 4.5 billion years from now.');
INSERT INTO public.galaxy VALUES (3, 'Antennae', 90, 12.00, 'Appearence is similar to the insect antennae.');
INSERT INTO public.galaxy VALUES (4, 'AnteBackward', 2, 99.99, 'It appears to rotate backwards, as the tips of the spiral arms point in the direction of rotation.');
INSERT INTO public.galaxy VALUES (5, 'Bear_Paw', 100, 15.50, 'It resembles a bear paw.');
INSERT INTO public.galaxy VALUES (6, 'black_eye', 0, 99.99, 'It has a spectacular dark band of absorbing dust in front of the galaxy bright nucleus.');


--
-- Data for Name: moon; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.moon VALUES (20, 'Crystaline_Cascade', 8, false, ' his moon is adorned with cascading crystalline formations, creating a sparkling and magical lunar lan');
INSERT INTO public.moon VALUES (1, 'Luminara_Crescent', 1, true, 'A moon with a crescent-shaped glow, casting ethereal and delicate light across its nocturnal landscape.');
INSERT INTO public.moon VALUES (3, 'Titanis_Veil', 3, true, 'A moon enveloped in a veil of mist, creating an otherworldly and mysterious atmosphere that captivates observers.');
INSERT INTO public.moon VALUES (5, 'Nocturna_Ember', 5, true, 'A moon that radiates a warm, ember-like glow, providing a comforting and enchanting illumination during the dark hours.');
INSERT INTO public.moon VALUES (7, 'Aurora_Harmony', 7, true, 'A moon where the auroras dance in harmony, painting the night sky with vibrant and celestial colors.');
INSERT INTO public.moon VALUES (9, 'Umbra_Serenity', 9, true, 'Known for its serene and tranquil shadows, this moon offers a peaceful respite in the cosmic ballet.');
INSERT INTO public.moon VALUES (11, 'Astralspire_Beacon', 11, true, 'A moon resembling a radiant beacon, guiding celestial travelers with its luminous and guiding presence.');
INSERT INTO public.moon VALUES (13, 'Nightaven_Luster', 1, true, 'A moon with a lustrous glow, illuminating the cosmic canvas with its subtle and enchanting radiance.');
INSERT INTO public.moon VALUES (15, 'Nebula_Tranquil', 3, true, 'A tranquil moon surrounded by a nebula-inspired aura, imparting a sense of calmness and serenity.');
INSERT INTO public.moon VALUES (17, 'Celestis_Glow', 5, true, 'A moon with a gentle and celestial glow, creating an atmosphere of quiet majesty in the cosmic expanse.');
INSERT INTO public.moon VALUES (19, 'Sable_Seraph', 7, true, 'A moon with a dark and mysterious beauty, like a celestial guardian with wings of shadow.');
INSERT INTO public.moon VALUES (2, 'Selene_Echo', 2, false, 'This moon resonates with echoes of ancient celestial myths, its surface reflecting the quiet mysteries of the night.');
INSERT INTO public.moon VALUES (4, 'Lunaris_Whispers', 4, false, 'This moon is known for its soft whispers, as if the very air carries the secrets of the cosmos in the stillness of the night.');
INSERT INTO public.moon VALUES (6, 'Celestia_Mirage', 6, false, 'This moon creates mesmerizing illusions across its surface, playing tricks with the light and shadow in the cosmic theater.');
INSERT INTO public.moon VALUES (8, 'Lunafrost_Haven', 8, false, 'A moon covered in frosty landscapes, casting a serene and icy ambiance in the moonlit expanse.');
INSERT INTO public.moon VALUES (10, 'Silvermist_Ecliptic', 10, false, 'A moon with a shimmering silver mist that traces the ecliptic path, creating a celestial spectacle.');
INSERT INTO public.moon VALUES (12, 'Stardust_Mirage', 12, false, 'This moon is surrounded by a stardust mirage, giving it a dreamlike and fantastical quality.');
INSERT INTO public.moon VALUES (14, 'Lunaris Cascade', 2, false, 'Characterized by cascading moonlit beams, this moon creates a breathtaking display as light spills across its surface.');
INSERT INTO public.moon VALUES (16, 'Selena_Dream', 4, false, 'This moon is said to embody the dreams of Selena, casting a soft and soothing light reminiscent of celestial reveries.');
INSERT INTO public.moon VALUES (18, 'Moonshadow_Oasis', 6, false, 'Marked by shadows and an oasis-like allure, this moon evokes a sense of mystery and allure.');


--
-- Data for Name: planet; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.planet VALUES (1, 'Terraforge', true, true, 4);
INSERT INTO public.planet VALUES (2, 'Aquarius', true, true, 4);
INSERT INTO public.planet VALUES (3, 'Pyronis', false, true, 5);
INSERT INTO public.planet VALUES (4, 'Verdantara', true, true, 5);
INSERT INTO public.planet VALUES (5, 'Zephyrion', false, false, 6);
INSERT INTO public.planet VALUES (6, 'Astralynx', false, true, 6);
INSERT INTO public.planet VALUES (7, 'Geodeon', false, true, 7);
INSERT INTO public.planet VALUES (8, 'Lunaris', true, true, 7);
INSERT INTO public.planet VALUES (9, 'Oceania', true, true, 8);
INSERT INTO public.planet VALUES (10, 'Celestria', true, false, 8);
INSERT INTO public.planet VALUES (11, 'Embera', false, true, 9);
INSERT INTO public.planet VALUES (12, 'Seraphara', true, true, 9);


--
-- Data for Name: star; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.star VALUES (4, 'Celestria', 1500, 1, 'A radiant star with a spectrum that shifts between brilliant hues, known for its mesmerizing celestial dance.');
INSERT INTO public.star VALUES (5, 'Nebula', 2000, 2, 'A star surrounded by swirling nebulae, creating a dynamic and ever-changing cosmic display.');
INSERT INTO public.star VALUES (6, 'Quasar', 3000, 3, 'A high-energy star emitting intense bursts of light and energy, akin to a celestial lighthouse in the vastness of space.');
INSERT INTO public.star VALUES (7, 'Stellara', 5000, 4, 'A fiery and luminous star, characterized by its vibrant flames that dance across the cosmic canvas.');
INSERT INTO public.star VALUES (8, 'Cosmos', 1000, 5, 'A star that appears like a glowing ember, casting a warm and comforting glow throughout its celestial neighborhood.');
INSERT INTO public.star VALUES (9, 'Astral', 6000, 6, 'A star with a gentle and serene luminosity, creating a peaceful ambiance in its cosmic surroundings.');


--
-- Name: alien_life_alien_life_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.alien_life_alien_life_id_seq', 3, true);


--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.galaxy_galaxy_id_seq', 6, true);


--
-- Name: moon_moon_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.moon_moon_id_seq', 20, true);


--
-- Name: planet_planet_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.planet_planet_id_seq', 12, true);


--
-- Name: star_star_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.star_star_id_seq', 9, true);


--
-- Name: alien_life alien_life_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.alien_life
    ADD CONSTRAINT alien_life_pkey PRIMARY KEY (alien_life_id);


--
-- Name: galaxy galaxy_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_name_key UNIQUE (name);


--
-- Name: galaxy galaxy_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_pkey PRIMARY KEY (galaxy_id);


--
-- Name: moon moon_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_name_key UNIQUE (name);


--
-- Name: moon moon_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_pkey PRIMARY KEY (moon_id);


--
-- Name: planet planet_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_name_key UNIQUE (name);


--
-- Name: planet planet_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_pkey PRIMARY KEY (planet_id);


--
-- Name: star star_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_name_key UNIQUE (name);


--
-- Name: star star_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_pkey PRIMARY KEY (star_id);


--
-- Name: alien_life unique_alien_name; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.alien_life
    ADD CONSTRAINT unique_alien_name UNIQUE (name);


--
-- Name: star fk_galaxy; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT fk_galaxy FOREIGN KEY (galaxy_id) REFERENCES public.galaxy(galaxy_id);


--
-- Name: moon fk_planet; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT fk_planet FOREIGN KEY (planet_id) REFERENCES public.planet(planet_id);


--
-- Name: planet fk_star; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT fk_star FOREIGN KEY (star_id) REFERENCES public.star(star_id);


--
-- PostgreSQL database dump complete
--
