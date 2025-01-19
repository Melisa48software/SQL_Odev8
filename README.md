# SQL_Odev8
lcw bootcamp sql 8.ödev reposudur.

-- 1. Employee Tablosunun Oluşturulması
CREATE TABLE employee (
    id INTEGER PRIMARY KEY,
    name VARCHAR(50),
    birthday DATE,
    email VARCHAR(100)
);

-- 2. Mockaroo Servisinden 50 Adet Veri Ekleniyor
INSERT INTO employee (id, name, birthday, email) VALUES
(1, 'John Doe', '1990-01-15', 'john.doe@example.com'),
(2, 'Jane Smith', '1985-07-22', 'jane.smith@example.com'),
(3, 'Michael Johnson', '1992-03-30', 'michael.johnson@example.com'),
(4, 'Emily Davis', '1980-11-05', 'emily.davis@example.com'),
(5, 'Sarah Brown', '1989-09-18', 'sarah.brown@example.com'),
(6, 'David Wilson', '1993-06-17', 'david.wilson@example.com'),
(7, 'Laura Lee', '1988-02-25', 'laura.lee@example.com'),
(8, 'Chris White', '1991-11-03', 'chris.white@example.com'),
(9, 'Olivia Harris', '1995-09-14', 'olivia.harris@example.com'),
(10, 'James Clark', '1987-10-28', 'james.clark@example.com'),
(11, 'Patricia Lewis', '1990-12-19', 'patricia.lewis@example.com'),
(12, 'William Walker', '1984-05-11', 'william.walker@example.com'),
(13, 'Thomas Allen', '1992-08-30', 'thomas.allen@example.com'),
(14, 'Sophia Young', '1994-01-22', 'sophia.young@example.com'),
(15, 'Benjamin Scott', '1983-07-29', 'benjamin.scott@example.com'),
(16, 'Amelia Martinez', '1990-03-13', 'amelia.martinez@example.com'),
(17, 'Henry King', '1992-10-06', 'henry.king@example.com'),
(18, 'Mason Harris', '1991-04-15', 'mason.harris@example.com'),
(19, 'Evelyn Green', '1989-08-25', 'evelyn.green@example.com'),
(20, 'Lucas Adams', '1993-09-30', 'lucas.adams@example.com'),
(21, 'Ava Nelson', '1986-06-23', 'ava.nelson@example.com'),
(22, 'Ethan Carter', '1994-02-17', 'ethan.carter@example.com'),
(23, 'Madison Roberts', '1992-11-10', 'madison.roberts@example.com'),
(24, 'Jackson Mitchell', '1987-04-12', 'jackson.mitchell@example.com'),
(25, 'Isabella Perez', '1991-08-19', 'isabella.perez@example.com'),
(26, 'Daniel Campbell', '1985-03-03', 'daniel.campbell@example.com'),
(27, 'Charlotte Sanchez', '1993-07-11', 'charlotte.sanchez@example.com'),
(28, 'Liam Evans', '1990-09-25', 'liam.evans@example.com'),
(29, 'Zoe Young', '1991-05-14', 'zoe.young@example.com'),
(30, 'Michael Roberts', '1989-11-28', 'michael.roberts@example.com'),
(31, 'Ella Martinez', '1992-02-22', 'ella.martinez@example.com'),
(32, 'Jackson Brown', '1994-12-04', 'jackson.brown@example.com'),
(33, 'Victoria Thomas', '1988-01-15', 'victoria.thomas@example.com'),
(34, 'Megan Moore', '1990-04-06', 'megan.moore@example.com'),
(35, 'Noah Taylor', '1984-10-01', 'noah.taylor@example.com'),
(36, 'Scarlett Evans', '1993-03-18', 'scarlett.evans@example.com'),
(37, 'Liam Lee', '1991-12-12', 'liam.lee@example.com'),
(38, 'Oliver Anderson', '1992-05-26', 'oliver.anderson@example.com'),
(39, 'Sophia Clark', '1987-07-04', 'sophia.clark@example.com'),
(40, 'Grace Harris', '1990-02-08', 'grace.harris@example.com'),
(41, 'Henry King', '1994-11-20', 'henry.king@example.com'),
(42, 'Carter White', '1985-10-18', 'carter.white@example.com'),
(43, 'Elijah Johnson', '1993-07-09', 'elijah.johnson@example.com'),
(44, 'Lily Turner', '1988-09-21', 'lily.turner@example.com'),
(45, 'Landon Scott', '1991-06-03', 'landon.scott@example.com'),
(46, 'Chloe Gonzalez', '1989-08-16', 'chloe.gonzalez@example.com'),
(47, 'Madeline Miller', '1990-01-23', 'madeline.miller@example.com'),
(48, 'Gabriel Williams', '1992-04-11', 'gabriel.williams@example.com'),
(49, 'Sofia Perez', '1987-12-05', 'sofia.perez@example.com'),
(50, 'Alice Walker', '1995-12-11', 'alice.walker@example.com');

-- 3. UPDATE İşlemleri

-- 3.1. Name Sütununa Göre Güncelleme
UPDATE employee
SET name = 'Johnathan Doe'
WHERE name = 'John Doe';

-- 3.2. Birthday Sütununa Göre Güncelleme
UPDATE employee
SET birthday = '1992-08-15'
WHERE birthday = '1985-07-22';

-- 3.3. Email Sütununa Göre Güncelleme
UPDATE employee
SET email = 'new.email@example.com'
WHERE email = 'sarah.brown@example.com';

-- 3.4. ID Sütununa Göre Güncelleme
UPDATE employee
SET name = 'Emily Davis Jr.'
WHERE id = 4;

-- 3.5. Birthday Sütununa Göre Güncelleme
UPDATE employee
SET birthday = '1987-03-05'
WHERE birthday = '1990-01-15';

-- 4. DELETE İşlemleri

-- 4.1. Name Sütununa Göre Silme
DELETE FROM employee
WHERE name = 'Johnathan Doe';

-- 4.2. Birthday Sütununa Göre Silme
DELETE FROM employee
WHERE birthday = '1992-08-15';

-- 4.3. Email Sütununa Göre Silme
DELETE FROM employee
WHERE email = 'new.email@example.com';

-- 4.4. ID Sütununa Göre Silme
DELETE FROM employee
WHERE id = 4;

-- 4.5. Birthday Sütununa Göre Silme
DELETE FROM employee
WHERE birthday = '1987-03-05';

