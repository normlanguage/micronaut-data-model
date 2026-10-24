# micronaut.data.model Skill

Use this skill to work with Norm module `micronaut.data.model` version 3. Use only declarations listed below.

## `micronaut.data.model`

Source: `CrudRepository.norm`

### `CrudRepository`

```norm
interface CrudRepository<E, ID> extends GenericRepository<E, ID>
```

Type parameters:

- `E`
- `ID`

#### `count`

```norm
Long count()
```

Returns: `Long`

#### `delete`

```norm
Void delete(E? arg0)
```

Parameters:

- `arg0`: `E?`

Returns: `Void`

#### `deleteAll`

```norm
Void deleteAll()
```

Returns: `Void`

#### `deleteById`

```norm
Void deleteById(ID? arg0)
```

Parameters:

- `arg0`: `ID?`

Returns: `Void`

#### `existsById`

```norm
Boolean existsById(ID? arg0)
```

Parameters:

- `arg0`: `ID?`

Returns: `Boolean`

#### `findAll`

```norm
JavaList<E>? findAll()
```

Returns: `JavaList<E>?`

#### `findById`

```norm
Optional<E>? findById(ID? arg0)
```

Parameters:

- `arg0`: `ID?`

Returns: `Optional<E>?`

#### `save`

```norm
S? save<S extends E>(S? arg0)
```

Type parameters:

- `S` extends `E`

Parameters:

- `arg0`: `S?`

Returns: `S?`

#### `saveAll`

```norm
JavaList<S>? saveAll<S extends E>(Function<Iterator<S>?()>? arg0)
```

Type parameters:

- `S` extends `E`

Parameters:

- `arg0`: `Function<Iterator<S>?()>?`

Returns: `JavaList<S>?`

## `micronaut.data.model`

Source: `DateCreated.norm`

### `DateCreated`

```norm
annotation DateCreated implements FieldTarget, FunctionTarget, RuntimeRetention
```

## `micronaut.data.model`

Source: `DateUpdated.norm`

### `DateUpdated`

```norm
annotation DateUpdated implements FieldTarget, FunctionTarget, RuntimeRetention
```

## `micronaut.data.model`

Source: `Dialect.norm`

### `Dialect`

```norm
enum Dialect
```

#### `ANSI`

```norm
ANSI
```

#### `H2`

```norm
H2
```

#### `MYSQL`

```norm
MYSQL
```

#### `ORACLE`

```norm
ORACLE
```

#### `POSTGRES`

```norm
POSTGRES
```

#### `SQLITE`

```norm
SQLITE
```

#### `SQL_SERVER`

```norm
SQL_SERVER
```

## `micronaut.data.model`

Source: `GeneratedValue.norm`

### `GeneratedValue`

```norm
annotation GeneratedValue implements TypeTarget, FieldTarget, FunctionTarget, RuntimeRetention
```

#### `value`

```norm
GeneratedValueType value
```

Type: `GeneratedValueType`

#### `GeneratedValue`

```norm
GeneratedValue(GeneratedValueType? value)
```

Parameters:

- `value`: `GeneratedValueType?`

## `micronaut.data.model`

Source: `GeneratedValueType.norm`

### `GeneratedValueType`

```norm
enum GeneratedValueType
```

#### `AUTO`

```norm
AUTO
```

#### `IDENTITY`

```norm
IDENTITY
```

#### `SEQUENCE`

```norm
SEQUENCE
```

#### `UUID`

```norm
UUID
```

## `micronaut.data.model`

Source: `Id.norm`

### `Id`

```norm
annotation Id implements TypeTarget, FieldTarget, FunctionTarget, ParameterTarget, RuntimeRetention, InheritedAnnotation
```

## `micronaut.data.model`

Source: `MappedEntity.norm`

### `MappedEntity`

```norm
annotation MappedEntity implements TypeTarget, FieldTarget, FunctionTarget, RuntimeRetention
```

#### `value`

```norm
String value
```

Type: `String`

#### `MappedEntity`

```norm
MappedEntity(String? value)
```

Parameters:

- `value`: `String?`

## `micronaut.data.model`

Source: `Page.norm`

### `Page`

```norm
interface Page<T> extends Slice<T>
```

Type parameters:

- `T`

#### `getContent`

```norm
JavaList<T>? getContent()
```

Returns: `JavaList<T>?`

#### `getNumberOfElements`

```norm
Integer getNumberOfElements()
```

Returns: `Integer`

#### `getTotalPages`

```norm
Integer getTotalPages()
```

Returns: `Integer`

#### `getTotalSize`

```norm
Long getTotalSize()
```

Returns: `Long`

#### `hasNext`

```norm
Boolean hasNext()
```

Returns: `Boolean`

#### `hasTotalSize`

```norm
Boolean hasTotalSize()
```

Returns: `Boolean`

#### `isEmpty`

```norm
Boolean isEmpty()
```

Returns: `Boolean`

## `micronaut.data.model`

Source: `Pageable.norm`

### `Pageable`

```norm
interface Pageable extends Sort
```

#### `getNumber`

```norm
Integer getNumber()
```

Returns: `Integer`

#### `getOffset`

```norm
Long getOffset()
```

Returns: `Long`

#### `getSize`

```norm
Integer getSize()
```

Returns: `Integer`

#### `isUnpaged`

```norm
Boolean isUnpaged()
```

Returns: `Boolean`

#### `next`

```norm
Pageable? next()
```

Returns: `Pageable?`

#### `previous`

```norm
Pageable? previous()
```

Returns: `Pageable?`

### `pageableFrom`

```norm
Pageable? pageableFrom(Integer arg0, Integer arg1)
```

Parameters:

- `arg0`: `Integer`
- `arg1`: `Integer`

Returns: `Pageable?`

## `micronaut.data.model`

Source: `PageableRepository.norm`

### `PageableRepository`

```norm
interface PageableRepository<E, ID> extends CrudRepository<E, ID>
```

Type parameters:

- `E`
- `ID`

#### `findAll`

```norm
Page<E>? findAll(Pageable? arg0)
```

Parameters:

- `arg0`: `Pageable?`

Returns: `Page<E>?`

## `micronaut.data.model.model`

Source: `model/Slice.norm`

### `Slice`

```norm
interface Slice<T> extends Iterable<T>
```

Type parameters:

- `T`

## `micronaut.data.model.model`

Source: `model/Sort.norm`

### `Sort`

```norm
interface Sort
```

## `micronaut.data.model.repository`

Source: `repository/GenericRepository.norm`

### `GenericRepository`

```norm
interface GenericRepository<E, ID>
```

Type parameters:

- `E`
- `ID`

