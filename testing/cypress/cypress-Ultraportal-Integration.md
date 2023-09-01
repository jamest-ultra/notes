      - name: Setup tmate session
        uses: mxschmitt/action-tmate@v3
		
      - run: |
          docker exec -it ultraportal-cypress-integration_database_1 bash
          mysql -u root
          create database ultraportal;
		  
      - name: run docker container
        run:  docker run -d --name docker -p 8080:80 my-docker-image
		
	  - name: Cypress run
        uses: cypress-io/github-action@v5
        continue-on-error: true
        with:
          command: npx cypress run --record
          record: true
          parallel: true
          browser: chrome
          working-directory: './src'
        env:
          CYPRESS_RECORD_KEY: ${{ secrets.CYPRESS_RECORD_KEY }}
