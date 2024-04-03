-- Tabela Book
INSERT INTO Book (title, Description, ReleaseYear, Status) VALUES 
('Harry Potter i Kamień Filozoficzny', 'Pierwszy tom serii o czarodzieju Harrym Potterze.', 1997, 'Available'),
('Władca Pierścieni: Drużyna Pierścienia', 'Pierwsza część epickiej sagi fantasy.', 1954, 'Available'),
('Zbrodnia i kara', 'Klasyczna powieść rosyjska opowiadająca historię Rodiona Raskolnikowa.', 1866, 'Available'),
('1984', 'Dystopijna wizja przyszłości, gdzie państwo totalitarne kontroluje wszystkie aspekty życia.', 1949, 'Available'),
('To', 'Przerażająca powieść o potworze, który poluje na dzieci w fikcyjnym miasteczku.', 1986, 'Available'),
('Mały Książę', 'Filozoficzna baśń o przyjaźni i miłości.', 1943, 'Available'),
('Mistrz i Małgorzata', 'Satyra na sowieckie społeczeństwo, opowiada o niespodziewanych gościach w Moskwie.', 1967, 'Available'),
('Duma i uprzedzenie', 'Romantyczna powieść obyczajowa, w której główna bohaterka Elizabeth Bennet poznaje Mr. Darcyego.', 1813, 'Available'),
('Martwe dusze', 'Satyra na rosyjskie społeczeństwo w czasach carskich.', 1842, 'Available'),
('Moby Dick', 'Epicka opowieść o kapitanie Achabie i jego obsesji na punkcie wieloryba.', 1851, 'Available');

-- Tabela Rent
INSERT INTO Rent (id_order, id_copy, data_rent, data_return, RentTime) VALUES 
(1, 1, '2024-03-01', '2024-03-08', 7),
(2, 2, '2024-03-02', '2024-03-09', 7),
(3, 3, '2024-03-03', '2024-03-10', 7),
(4, 4, '2024-03-04', '2024-03-11', 7),
(5, 5, '2024-03-05', '2024-03-12', 7),
(6, 6, '2024-03-06', '2024-03-13', 7),
(7, 7, '2024-03-07', '2024-03-14', 7),
(8, 8, '2024-03-08', '2024-03-15', 7),
(9, 9, '2024-03-09', '2024-03-16', 7),
(10, 10, '2024-03-10', '2024-03-17', 7);

-- Tabela Orders
INSERT INTO Orders (id_Order, rent, data, ReceivingTime, id_User, id_copy) VALUES 
(1, 'true', '2024-03-01', '2024-03-08', 1, 1),
(2, 'true', '2024-03-02', '2024-03-09', 2, 2),
(3, 'true', '2024-03-03', '2024-03-10', 3, 3),
(4, 'true', '2024-03-04', '2024-03-11', 4, 4),
(5, 'true', '2024-03-05', '2024-03-12', 5, 5),
(6, 'true', '2024-03-06', '2024-03-13', 6, 6),
(7, 'true', '2024-03-07', '2024-03-14', 7, 7),
(8, 'true', '2024-03-08', '2024-03-15', 8, 8),
(9, 'true', '2024-03-09', '2024-03-16', 9, 9),
(10, 'true', '2024-03-10', '2024-03-17', 10, 10);

-- Tabela User
INSERT INTO User (Status, Login, Type, LastName, FirstName, PWIndex, rent, Sms, Mail) VALUES 
('Active', 'user1', 'Student', 'Kowalski', 'Jan', 123456, 'true', 1, 'user1@example.com'),
('Active', 'user2', 'Teacher', 'Nowak', 'Anna', 234567, 'true', 1, 'user2@example.com'),
('Active', 'user3', 'Student', 'Wiśniewski', 'Katarzyna', 345678, 'true', 1, 'user3@example.com'),
('Active', 'user4', 'Teacher', 'Wójcik', 'Piotr', 456789, 'true', 1, 'user4@example.com'),
('Active', 'user5', 'Student', 'Kowalczyk', 'Maria', 567890, 'true', 1, 'user5@example.com'),
('Active', 'user6', 'Teacher', 'Lewandowski', 'Magdalena', 678901, 'true', 1, 'user6@example.com'),
('Active', 'user7', 'Student', 'Kamiński', 'Tomasz', 789012, 'true', 1, 'user7@example.com'),
('Active', 'user8', 'Teacher', 'Jankowski', 'Marcin', 890123, 'true', 1, 'user8@example.com'),
('Active', 'user9', 'Student', 'Woźniak', 'Agnieszka', 901234, 'true', 1, 'user9@example.com'),
('Active', 'user10', 'Teacher', 'Mazur', 'Marek', 123456, 'true', 1, 'user10@example.com');

-- Tabela Copy
INSERT INTO Copy (Status, use, id_library, id_book) VALUES 
('Available', 1, 1, 1),
('Available', 1, 1, 2),
('Available', 1, 1, 3),
('Available', 1, 1, 4),
('Available', 1, 1, 5),
('Available', 1, 1, 6),
('Available', 1, 1, 7),
('Available', 1, 1, 8),
('Available', 1, 1, 9),
('Available', 1, 1, 10);