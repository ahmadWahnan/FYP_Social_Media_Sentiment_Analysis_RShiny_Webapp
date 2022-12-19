library(shiny)
library(shinythemes)
library(ggplot2)


ui <- fluidPage(
  theme = shinytheme("paper"),
  navbarPage(
    "Twitter Sentiment Analysis",
    sidebarLayout(
      sidebarPanel(
        helpText("Explore the general sentiment of brand, topic, celebrities or events on Twitter"),
        textInput("inputKeyword","Query Keywords",""),
        
        sliderInput("inputTweetQueryNumber","Maximum number of Tweets",min = 1, max = 1000, value = 100),
        
        sliderInput("inputMinimumLikes","Minimum Likes",min = 0, max = 100, value = 0),
        
        sliderInput("inputMinimumReplies","Minimum Replies",min = 0, max = 100, value = 0),
        
        sliderInput("inputMinimumRetweets","Minimum Retweets",min = 0, max = 100, value = 0),
        
        selectInput("inputType","Tweet Type", 
                    choices = list("Recently Posted" = "recent", 
                                   "Popular" = "popular", 
                                   "Mixed" = "mixed"
                    ), 
                    selected = "recent"),
        
        selectInput("inputLanguage","Tweet Language", 
                    choices = list("English" = "en", "Malay" = "my"), 
                    selected = "en"),
        
        checkboxInput("inputIncludeLinks","Include Links ", value = FALSE),
        
        checkboxInput("inputIncludeReplies","Include Replies ", value = FALSE),
        
        checkboxInput("inputIncludeRTS","Include Retweets ", value = FALSE),
        
        actionButton("update","Analyze")
      ),
      
      mainPanel(
        tabsetPanel(type = "tabs",
                    tabPanel("Raw",
                             DT::dataTableOutput("tableRaw")
                    ),
                    
                    tabPanel("VADER",
                             plotOutput("plotVADER"),
                             plotOutput("plotVADER2"),
                             DT::dataTableOutput("tableVADER")
                    ),
                    
                    tabPanel("sentimentr",
                             plotOutput("plotGI"),
                             DT::dataTableOutput("tableSentimentr")
                    ),
                    
                    tabPanel("SentimentAnalysis",
                             DT::dataTableOutput("tableSA")
                    ),
                    
                    tabPanel("Emotion",
                             plotOutput("plotEmotion1"),
                             plotOutput("plotEmotion2"),
                             DT::dataTableOutput("tableEmotion")
                    )
        )
        
      )
    )
  )
)
