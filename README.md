# Newcoding
const { cyan } = require("color-name")
const { select } = require("async")

describe('my third demo',function()

{
    
    it('first method',function(){
        cy.visit("https://www.vantashala.com/")
       // cy.visit("http://www.vantashala.com")
        cy.wait(2000)
        //cy.get('.v-btn__content > .dropdown-select')
       // cy.get('.v-btn__content ').contains('USA')   
      // cy.get('v-btn_content').select('USA').click()  
        //cy.get('.v-btn_content').select('dropdown-select')=="USA"
       // cy.get('select').select('USA').should('have.value','USA')
        cy.get('.dropdown-select ma-auto')
              .select('USA').should('have.value', 'USA')
    })
})
