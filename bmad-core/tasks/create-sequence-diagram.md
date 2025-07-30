# Create Sequence Diagram

## Purpose
Create detailed sequence diagrams for specific use cases to visualize system interactions and component relationships.

## When to Use
- During architecture design to clarify component interactions
- When implementing complex workflows that span multiple services
- To document API interactions and data flow
- For troubleshooting complex system behaviors
- When onboarding new team members to system architecture

## Prerequisites
- Project architecture document (docs/architecture.md)
- Clear understanding of the use case to be diagrammed
- Component definitions and API specifications

## Workflow

### Step 1: Use Case Analysis
1. **Identify the Use Case**
   - Review the user's description of the sequence to be diagrammed
   - Clarify the scope and boundaries of the interaction
   - Identify the primary actor(s) and system components involved

2. **Gather Context**
   - Review existing architecture documentation
   - Identify relevant components, services, and APIs
   - Understand data flow and business logic requirements

3. **Define Interaction Scope**
   - Determine the start and end points of the sequence
   - Identify all participating components/systems
   - Clarify any external dependencies or integrations

### Step 2: Component Identification
1. **List All Participants**
   - Primary actors (users, external systems)
   - Internal system components
   - External services and APIs
   - Data stores and message queues

2. **Define Component Responsibilities**
   - Clarify what each component does in the sequence
   - Identify the interfaces and methods being called
   - Document any state changes or side effects

### Step 3: Sequence Flow Design
1. **Map the Interaction Flow**
   - Define the chronological order of interactions
   - Identify synchronous vs asynchronous operations
   - Document error handling and alternative flows
   - Include timing considerations if relevant

2. **Handle Edge Cases**
   - Consider failure scenarios and recovery
   - Document retry logic and circuit breakers
   - Include timeout and error response handling

### Step 4: Diagram Creation
1. **Create Mermaid Sequence Diagram**
   - Use the sequence-diagram-tmpl.yaml template
   - Follow Mermaid sequence diagram syntax
   - Include all identified participants and interactions
   - Add appropriate notes and comments

2. **Validate the Diagram**
   - Ensure all interactions are properly represented
   - Verify component names match architecture documentation
   - Check that the flow is logical and complete

### Step 5: Documentation
1. **Add Context and Notes**
   - Provide a clear description of the use case
   - Document any assumptions or constraints
   - Include relevant business rules or requirements
   - Add references to related documentation

2. **Integration with Architecture**
   - Update architecture document if new insights are discovered
   - Link the sequence diagram to relevant components
   - Ensure consistency with existing documentation

## Output
- Mermaid sequence diagram in markdown format
- Detailed description of the use case and interactions
- Integration notes for architecture documentation
- Any discovered architectural improvements or concerns

## Quality Checklist
- [ ] All relevant components are included
- [ ] Interaction flow is logical and complete
- [ ] Error handling and edge cases are considered
- [ ] Component names match architecture documentation
- [ ] Diagram syntax is valid and renders correctly
- [ ] Context and assumptions are clearly documented
- [ ] Integration with existing documentation is complete

## Example Usage

create-sequence-diagram "User login flow including OAuth integration and session management"