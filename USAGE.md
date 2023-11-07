<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	"log"
	petstore "petstore/v2"
)

func main() {
	s := petstore.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->