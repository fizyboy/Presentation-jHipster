##  Spring Data JPA

- Simple CRUD Repositories
- (findAll, create, update, delete, and more)
- Dynamic Finders 

```java
public interface AttendeeRepository extends JpaRepository<Attendee, Long> {

	List<Attendee> findByOrderByNameDesc();
    
	List<Attendee> findByNameOrderByNameAsc(String name);
    
	List<Attendee> findByOrderByNameAsc();

}

```



note:
    Put your speaker notes here.
    You can see them pressing 's'.
