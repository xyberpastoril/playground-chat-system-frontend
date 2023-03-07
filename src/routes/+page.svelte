<script>
    import { onMount } from 'svelte';
    import { Form, FormGroup, Label, Input, Button, Container, Row, Col, CardBody, Card, InputGroup } from 'sveltestrap';
    
    
    
    function handleSubmit(event) {
        // event.preventDefault();
        // const formData = new FormData(event.target);
        // const email = formData.get('email');
        // const password = formData.get('password');
        // console.log(`Email: ${email}, Password: ${password}`);
        // perform any additional logic or API calls here
    }
    
    onMount(() => {
        
    });
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<Container fluid class="d-flex p-0" style="height: 100vh;">
	<Row class="p-0 m-0" style="width: 100%">
		<Col md="3" class="p-0" style="background-color:#eee">
			<div class="px-3 pt-3">
				<h4>Demo: Chat System</h4>
				<Form>
					<FormGroup>
						<Input type="text" placeholder="Search..."></Input>
					</FormGroup>
					<Button color="primary">Search</Button>
				</Form>
				<hr>
			</div>
			<div class="px-3">
				<h4>Conversations</h4>
				<ul>
					<li>Conversation 1</li>
					<li>Conversation 2</li>
					<li>Conversation 3</li>
				</ul>
			</div>
		</Col>
		<Col md="9" class="d-flex flex-column justify-content-end p-0">
			<div class="px-3 pt-3">
				<h4>Conversation View</h4>
			</div>
			<div style="max-height: calc(100vh - 92px - 40px);" class="pt-3 pb-4 flex-grow-1 overflow-auto d-flex flex-column flex-column-reverse">
				<div class="px-3">
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-end align-items-center">
						<div class="bg-primary text-light p-2 rounded my-2">
						Outbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Another inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-end align-items-center">
						<div class="bg-primary text-light p-2 rounded my-2">
						Outbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Another inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-end align-items-center">
						<div class="bg-primary text-light p-2 rounded my-2">
						Outbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Another inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-end align-items-center">
						<div class="bg-primary text-light p-2 rounded my-2">
						Outbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Another inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Inbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-end align-items-center">
						<div class="bg-primary text-light p-2 rounded my-2">
						Outbound message goes here...
						</div>
					</div>
					<div class="d-flex justify-content-start align-items-center">
						<div class="border border-dark bg-light text-dark p-2 rounded my-2">
						Another inbound message goes here...
						</div>
					</div>
				</div>
			</div>
			<Form class="p-3" style="background-color:#ddd">
				<InputGroup>
					<Input type="text" placeholder="Type a message..."></Input>
					<Button color="primary">Send</Button>
				</InputGroup>
			</Form>
		</Col>		  
	</Row>
</Container>
