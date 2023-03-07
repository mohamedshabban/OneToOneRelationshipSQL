# OneToOneRelationshipSQL
One to One Relationship (1:1)

CREATE TABLE Country
(
CountryID INT IDENTITY PRIMARY KEY,
Name VARCHAR(100),
);

CREATE TABLE Capital
(
CapitalID INT PRIMARY KEY,
Name VARCHAR(100),
FOREIGN KEY(CapitalID) REFERENCES Country(CountryID)
);


INSERT INTO Country (Name)
VALUES ('Nigeria');
INSERT INTO Country (Name)
VALUES ('Ghana');

INSERT INTO Country (Name)
VALUES ('South Africa');


