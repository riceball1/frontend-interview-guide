<template>
  <div class="container">
    <Header />

    <CBox p="12" mb="32">

      <CHeading text-align="left" as="h2"> Frontend Systems Design </CHeading>
      <CFlex justify="center" direction="column">
        <CHeading as="h3">Introduction</CHeading>
        <CText>
          Traditional system design interviews may involve the distributed system,
          which includes server, load balancer, databases, etc. However, for
          frontend system design interviews, the focus is more on the client and
          API design, rather than what goes on in the backend.
        </CText>
        <CText>
          Due to the open-ended types of problems inherit in system design,
          there's not necessary a right answer, however there are better answers
          than others. Examples of types of problems for frontend system design
          interviews, may include: autocomplete, image carousel, news feed, emoji
          reaction to a chat message.
        </CText>
        <CText>
          System design interviews mainly focuses on the presentation of ideas,
          but it shouldn't involve implementation of code. The interviewer is
          there to give you support, but it's expected for the interviewee to
          drive the system design presentation. Sometimes you may find the
          interviewer is bias towards a particular part of the system, focus your
          attention there, and make sure to focus on what you do know.
        </CText>
        <CText>
          The fundamental traits that make up a frontend system design doesn't
          look that much different from any other system design. However, the
          things that should be considered when working on frontend system design
          may include:
        </CText>
  
          <ul class="list">
            <li>Gather Requirements</li>
            <li>Scope</li>
            <li>Tech Choices</li>
            <li>Component Architecture/High Level Design</li>
            <li>Data API and protocCLists</li>
            <li>Optimizations and Deep Dive/ Low Level Design</li>
          </ul>
     
  
        <CHeading as="h3">Gather Requirements</CHeading>
        <CText>
          When gathering the requirements, it's important to understand the goal
          and the problem statement. Make sure to ask clarifying questions about
          what potentially should part of the requirements for the system design.
        </CText>
        <CHeading as="h3">Scope</CHeading>
        <CText>
          Determine what part of the system to focus on, such as the core
          features, extended requirements, and out of scope.
        </CText>
        <h3>Tech Choices</h3>
        <CText>
          Here it would be good to consider the trade offs of particular
          technologies and approaches to use
        </CText>
        <CHeading as="h3">Component Architecture/High Level Design</CHeading>
        <CHeading as="h3">Data API and protocols</CHeading>
        <CHeading as="h3">Optimizations and Deep Dive/ Low Level Design</CHeading>
      </CFlex>
    </CBox>

    <Footer />
  </div>
</template>

<script lang="js">
import { CBox, CFlex, CHeading, CText, CListItem, CList } from "@chakra-ui/vue";

export default {
  name: "system",
}
</script>
