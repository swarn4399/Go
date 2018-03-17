package main

import (
	"net/http"
	"log"
	"time"
	"io/ioutil"
	"fmt"
)

func main()  {
	url := "https://dog.ceo/api/breeds/list/all"
	req, _ := http.NewRequest(http.MethodGet, url, nil)
	//if err != nil {
	//	log.Fatal(err)
	//}
	spaceClient := http.Client{
		Timeout: time.Second * 1000, // Maximum of 2 secs
	}
	res, getErr := spaceClient.Do(req)
	if getErr != nil {
		log.Fatal(getErr)
	}
	body, readErr := ioutil.ReadAll(res.Body)
	if readErr != nil {
		log.Fatal(readErr)
	}
	fmt.Println(string(body))
	
}
