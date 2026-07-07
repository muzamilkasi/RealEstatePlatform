# Database Design

## Planned Tables

- Users
- | Column          | Type         | Description        |
| --------------- | ------------ | ------------------ |
| Id              | UUID         | Primary Key        |
| FirstName       | VARCHAR(100) | User's first name  |
| LastName        | VARCHAR(100) | User's last name   |
| Email           | VARCHAR(255) | Unique email       |
| PhoneNumber     | VARCHAR(20)  | Contact number     |
| PasswordHash    | TEXT         | Encrypted password |
| ProfileImageUrl | TEXT         | Profile picture    |
| RoleId          | UUID         | Links to Roles     |
| CreatedAt       | TIMESTAMP    | Record creation    |
| UpdatedAt       | TIMESTAMP    | Last update        |

- Roles
| Column | Type        |
| ------ | ----------- |
| Id     | UUID        |
| Name   | VARCHAR(50) |

- Properties
| Column         | Type         |
| -------------- | ------------ |
| Id             | UUID         |
| Title          | VARCHAR(200) |
| Description    | TEXT         |
| Price          | DECIMAL      |
| Bedrooms       | INTEGER      |
| Bathrooms      | INTEGER      |
| AreaSize       | DECIMAL      |
| Address        | TEXT         |
| Latitude       | DECIMAL      |
| Longitude      | DECIMAL      |
| Purpose        | VARCHAR(20)  |
| PropertyTypeId | UUID         |
| AreaId         | UUID         |
| UserId         | UUID         |
| CreatedAt      | TIMESTAMP    |
| UpdatedAt      | TIMESTAMP    |


- PropertyImages
- PropertyTypes
- Cities
| Id     | UUID      | Primary Key |
| Name     | VARCHAR(200)      | Name of City |
- Areas
- Favorites
- Messages